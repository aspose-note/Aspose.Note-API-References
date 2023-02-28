---
title: Image.Bytes
second_title: Aspose.Note per .NET API Reference
description: Image proprietà. Ottiene larchivio dati immagine.
type: docs
weight: 50
url: /it/net/aspose.note/image/bytes/
---
## Image.Bytes property

Ottiene l'archivio dati immagine.

```csharp
public byte[] Bytes { get; }
```

### Esempi

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

### Guarda anche

* class [Image](../)
* spazio dei nomi [Aspose.Note](../../image/)
* assemblea [Aspose.Note](../../../)


