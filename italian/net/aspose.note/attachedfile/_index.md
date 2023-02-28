---
title: Class AttachedFile
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.AttachedFile classe. Rappresenta un file allegato.
type: docs
weight: 10
url: /it/net/aspose.note/attachedfile/
---
## AttachedFile class

Rappresenta un file allegato.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AttachedFile](attachedfile/#constructor)() | Inizializza una nuova istanza di`AttachedFile` classe. |
| [AttachedFile](attachedfile/#constructor_6)(string, Stream) | Inizializza una nuova istanza di`AttachedFile` classe. |
| [AttachedFile](attachedfile/#constructor_7)(string, Stream, ImageFormat) | Inizializza una nuova istanza di`AttachedFile` classe. |
| [AttachedFile](attachedfile/#constructor_8)(string, Stream, Stream, ImageFormat) | Inizializza una nuova istanza di`AttachedFile` classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment/) { get; set; } | Ottiene o imposta l'allineamento. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription/) { get; set; } | Ottiene o imposta un corpo un testo alternativo per l'icona del file allegato. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle/) { get; set; } | Ottiene o imposta un titolo di testo alternativo per l'icona del file allegato. |
| [Bytes](../../aspose.note/attachedfile/bytes/) { get; } | Ottiene i dati binari per un file incorporato. |
| [Document](../../aspose.note/node/document/) { get; } | Ottiene il documento del nodo. |
| [Extension](../../aspose.note/attachedfile/extension/) { get; } | Ottiene l'estensione di un file incorporato. |
| [FileName](../../aspose.note/attachedfile/filename/) { get; } | Ottiene il nome del file incorporato. |
| [FilePath](../../aspose.note/attachedfile/filepath/) { get; } | Ottiene il percorso del file originale. |
| [Height](../../aspose.note/attachedfile/height/) { get; } | Ottiene l'altezza originale dell'icona del file incorporato. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset/) { get; set; } | Ottiene o imposta l'offset orizzontale. |
| [Icon](../../aspose.note/attachedfile/icon/) { get; } | Ottiene i dati binari per l'icona associata al file incorporato. |
| [IconExtension](../../aspose.note/attachedfile/iconextension/) { get; } | Ottiene l'estensione dell'icona. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Ottiene un valore che indica se questo nodo è composto. Se vero il nodo può avere nodi figli. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout/) { get; set; } | Ottiene o imposta un valore che indica se la visualizzazione del file è stampata. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser/) { get; set; } | Ottiene o imposta un valore che indica se il valore della dimensione dell'icona è stato esplicitamente aggiornato dall'utente. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime/) { get; set; } | Ottiene o imposta l'ora dell'ultima modifica. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight/) { get; set; } | Ottiene o imposta l'altezza massima per visualizzare l'icona del file incorporato. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth/) { get; set; } | Ottiene o imposta la larghezza massima per visualizzare l'icona del file incorporato. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Ottiene il nodo successivo allo stesso livello di albero dei nodi. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Ottiene il tipo di nodo. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Ottiene il nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Ottiene il nodo precedente allo stesso livello dell'albero dei nodi. |
| [Tags](../../aspose.note/attachedfile/tags/) { get; } | Ottiene l'elenco di tutti i tag di un paragrafo. |
| [Text](../../aspose.note/attachedfile/text/) { get; set; } | Ottiene o imposta la rappresentazione testuale del file incorporato. La stringa NON DEVE contenere caratteri con valore 10 (line feed) o 13 (carriage return). |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset/) { get; set; } | Ottiene o imposta l'offset verticale. |
| [Width](../../aspose.note/attachedfile/width/) { get; } | Ottiene la larghezza originale dell'icona del file incorporato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept/)(DocumentVisitor) | Accetta il visitatore del nodo. |

### Esempi

Mostra come ottenere il contenuto di un file allegato.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Attachments();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Ottieni un elenco di nodi di file allegati
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Itera attraverso tutti i nodi
foreach (AttachedFile file in nodes)
{
    // Carica il file allegato a un oggetto stream
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Crea un file locale
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Copia il flusso di file
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Mostra come aggiungere un file a un documento usando filepath.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Inizializza l'oggetto della classe AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Aggiungi file allegato
outlineElem.AppendChildLast(attachedFile);

// Aggiungi nodo elemento contorno
outline.AppendChildLast(outlineElem);

// Aggiungi nodo di contorno
page.AppendChildLast(outline);

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Mostra come aggiungere un file da uno stream a un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Inizializza l'oggetto della classe AttachedFile e passa anche il suo percorso dell'icona
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Aggiungi file allegato
    outlineElem.AppendChildLast(attachedFile);
}

// Aggiungi nodo elemento contorno
outline.AppendChildLast(outlineElem);

// Aggiungi nodo di contorno
page.AppendChildLast(outline);

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### Guarda anche

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


