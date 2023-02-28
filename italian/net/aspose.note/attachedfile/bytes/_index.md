---
title: AttachedFile.Bytes
second_title: Aspose.Note per .NET API Reference
description: AttachedFile proprietà. Ottiene i dati binari per un file incorporato.
type: docs
weight: 50
url: /it/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Ottiene i dati binari per un file incorporato.

```csharp
public byte[] Bytes { get; }
```

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

### Guarda anche

* class [AttachedFile](../)
* spazio dei nomi [Aspose.Note](../../attachedfile/)
* assemblea [Aspose.Note](../../../)


