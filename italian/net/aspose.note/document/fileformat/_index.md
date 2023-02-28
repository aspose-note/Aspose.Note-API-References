---
title: Document.FileFormat
second_title: Aspose.Note per .NET API Reference
description: Document proprietà. Ottiene il formato file OneNote 2010 OneNote Online.
type: docs
weight: 60
url: /it/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

Ottiene il formato file (OneNote 2010, OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

### Esempi

Mostra come ottenere il formato file di un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Elabora OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Elabora OneNote online
        break;
}
```

### Guarda anche

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* spazio dei nomi [Aspose.Note](../../document/)
* assemblea [Aspose.Note](../../../)


