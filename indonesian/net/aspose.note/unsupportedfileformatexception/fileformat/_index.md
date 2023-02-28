---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note untuk Referensi .NET API
description: UnsupportedFileFormatException Properti. Mendapat format file dari data yang diteruskan jika terdeteksi.
type: docs
weight: 10
url: /id/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

Mendapat format file dari data yang diteruskan jika terdeteksi.

```csharp
public FileFormat FileFormat { get; }
```

### Contoh

Memperlihatkan cara memeriksa apakah pemuatan dokumen gagal karena format OneNote 2007 tidak didukung.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

### Lihat juga

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* ruang nama [Aspose.Note](../../unsupportedfileformatexception/)
* perakitan [Aspose.Note](../../../)


