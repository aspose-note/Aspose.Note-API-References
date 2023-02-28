---
title: Document.FileFormat
second_title: Aspose.Note untuk Referensi .NET API
description: Document Properti. Mendapatkan format file OneNote 2010 OneNote Online.
type: docs
weight: 60
url: /id/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

Mendapatkan format file (OneNote 2010, OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

### Contoh

Menunjukkan cara mendapatkan format file dari suatu dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Proses OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Proses OneNote Online
        break;
}
```

### Lihat juga

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


