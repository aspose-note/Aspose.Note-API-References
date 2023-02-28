---
title: Class UnsupportedFileFormatException
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.UnsupportedFileFormatException kelas. Dilempar saat dokumen dimuat saat format file tidak dikenali atau tidak didukung oleh Aspose.Note.
type: docs
weight: 990
url: /id/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

Dilempar saat dokumen dimuat, saat format file tidak dikenali atau tidak didukung oleh Aspose.Note.

```csharp
public class UnsupportedFileFormatException : Exception
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | Mendapat format file dari data yang diteruskan jika terdeteksi. |

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

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


