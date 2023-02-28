---
title: Image.LastModifiedTime
second_title: Aspose.Note per .NET API Reference
description: Image proprietà. Ottiene o imposta lora dellultima modifica.
type: docs
weight: 130
url: /it/net/aspose.note/image/lastmodifiedtime/
---
## Image.LastModifiedTime property

Ottiene o imposta l'ora dell'ultima modifica.

```csharp
public DateTime LastModifiedTime { get; set; }
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

### Guarda anche

* class [Image](../)
* spazio dei nomi [Aspose.Note](../../image/)
* assemblea [Aspose.Note](../../../)


