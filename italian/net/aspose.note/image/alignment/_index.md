---
title: Image.Alignment
second_title: Aspose.Note per .NET API Reference
description: Image proprietà. Ottiene o imposta lallineamento.
type: docs
weight: 20
url: /it/net/aspose.note/image/alignment/
---
## Image.Alignment property

Ottiene o imposta l'allineamento.

```csharp
public HorizontalAlignment Alignment { get; set; }
```

### Esempi

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

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* spazio dei nomi [Aspose.Note](../../image/)
* assemblea [Aspose.Note](../../../)


