---
title: Image.Height
second_title: Aspose.Note per .NET API Reference
description: Image proprietà. Ottiene o imposta laltezza. Questa è laltezza reale dellimmagine nel documento MS OneNote.
type: docs
weight: 90
url: /it/net/aspose.note/image/height/
---
## Image.Height property

Ottiene o imposta l'altezza. Questa è l'altezza reale dell'immagine nel documento MS OneNote.

```csharp
public float Height { get; set; }
```

### Esempi

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

### Guarda anche

* class [Image](../)
* spazio dei nomi [Aspose.Note](../../image/)
* assemblea [Aspose.Note](../../../)


