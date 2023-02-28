---
title: Class Image
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Image classe. Rappresenta unimmagine.
type: docs
weight: 250
url: /it/net/aspose.note/image/
---
## Image class

Rappresenta un'immagine.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Image](image/#constructor)() | Inizializza una nuova istanza di`Image` classe. |
| [Image](image/#constructor_4)(string, Stream) | Inizializza una nuova istanza di`Image` classe. |
| [Image](image/#constructor_5)(string, string, string) | Inizializza una nuova istanza di`Image` classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | Ottiene o imposta l'allineamento. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | Ottiene o imposta un corpo come testo alternativo per l'immagine. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | Ottiene o imposta un titolo di testo alternativo per l'immagine. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | Ottiene l'archivio dati immagine. |
| [Document](../../aspose.note/node/document/) { get; } | Ottiene il documento del nodo. |
| [FileName](../../aspose.note/image/filename/) { get; } | Ottiene il nome del file. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | Ottiene il percorso del file immagine. |
| [Format](../../aspose.note/image/format/) { get; } | Ottiene il formato dell'immagine. |
| [Height](../../aspose.note/image/height/) { get; set; } | Ottiene o imposta l'altezza. Questa è l'altezza reale dell'immagine nel documento MS OneNote. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | Ottiene o imposta l'offset orizzontale. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | Ottiene o imposta il collegamento ipertestuale associato all'immagine. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | Ottiene se l'immagine è un'immagine di sfondo. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Ottiene un valore che indica se questo nodo è composto. Se vero il nodo può avere nodi figli. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | Ottiene o imposta l'ora dell'ultima modifica. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Ottiene il nodo successivo allo stesso livello di albero dei nodi. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Ottiene il tipo di nodo. |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | Ottiene l'altezza originale. Questa è la larghezza originale dell'immagine, prima del ridimensionamento. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | Ottiene la larghezza originale. Questa è la larghezza originale dell'immagine, prima del ridimensionamento. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Ottiene il nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Ottiene il nodo precedente allo stesso livello dell'albero dei nodi. |
| [Tags](../../aspose.note/image/tags/) { get; } | Ottiene l'elenco di tutti i tag di un paragrafo. |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | Ottiene o imposta l'offset verticale. |
| [Width](../../aspose.note/image/width/) { get; set; } | Ottiene o imposta la larghezza. Questa è la larghezza reale dell'immagine nel documento MS OneNote. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | Accetta il visitatore del nodo. |

### Esempi

Mostra come associare un collegamento ipertestuale a un'immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Mostra come impostare la descrizione del testo per un'immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

Mostra come ottenere un'immagine da un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni tutti i nodi Immagine
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Salva i byte dell'immagine in un file
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Mostra come ottenere le meta informazioni dell'immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni tutti i nodi Immagine
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

Mostra come aggiungere una nuova immagine con tag.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Carica un'immagine
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Inserisci l'immagine nel nodo del documento
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Aggiungi nodo elemento contorno
outline.AppendChildLast(outlineElem);

// Aggiungi nodo di contorno
page.AppendChildLast(outline);

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

Mostra come aggiungere un'immagine da un file a un documento con proprietà definite dall'utente.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Carica il documento dal flusso.
Document doc = new Document(dataDir + "Aspose.one");

// Ottieni la prima pagina del documento.
Aspose.Note.Page page = doc.FirstChild;

// Carica un'immagine dal file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Modifica le dimensioni dell'immagine in base alle tue esigenze (opzionale).
                              Width = 100,
                              Height = 100,

                              // Imposta la posizione dell'immagine nella pagina (opzionale).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Imposta l'allineamento dell'immagine
                              Alignment = HorizontalAlignment.Right
                          };

// Aggiungi l'immagine alla pagina.
page.AppendChildLast(image);
```

Mostra come aggiungere un'immagine dallo stream a un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Carica la seconda immagine utilizzando il nome, l'estensione e il flusso dell'immagine.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Imposta l'allineamento dell'immagine
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Mostra come aggiungere un'immagine da un file a un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe Outline e imposta le proprietà di offset
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Carica un'immagine dal percorso del file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Imposta l'allineamento dell'immagine
                              Alignment = HorizontalAlignment.Right
                          };

// Aggiungi immagine
outlineElem.AppendChildLast(image);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem);

// Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi nodo Pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Guarda anche

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


