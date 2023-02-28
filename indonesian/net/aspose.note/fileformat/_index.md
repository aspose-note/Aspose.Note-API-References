---
title: Enum FileFormat
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.FileFormat enum. Merupakan format file OneNote.
type: docs
weight: 90
url: /id/net/aspose.note/fileformat/
---
## FileFormat enumeration

Merupakan format file OneNote.

```csharp
public enum FileFormat
```

### Nilai

| Nama | Nilai | Keterangan |
| --- | --- | --- |
| Unknown | `0` | Format file tidak dikenal. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote Online. |

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


