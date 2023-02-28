---
title: AttachedFile.Bytes
second_title: Aspose.Note untuk Referensi .NET API
description: AttachedFile Properti. Mendapatkan data biner untuk file yang disematkan.
type: docs
weight: 50
url: /id/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Mendapatkan data biner untuk file yang disematkan.

```csharp
public byte[] Bytes { get; }
```

### Contoh

Menunjukkan cara mendapatkan konten dari file terlampir.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Dapatkan daftar node file terlampir
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Iterasi melalui semua node
foreach (AttachedFile file in nodes)
{
    // Memuat file terlampir ke objek aliran
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Buat file lokal
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Salin aliran file
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### Lihat juga

* class [AttachedFile](../)
* ruang nama [Aspose.Note](../../attachedfile/)
* perakitan [Aspose.Note](../../../)


