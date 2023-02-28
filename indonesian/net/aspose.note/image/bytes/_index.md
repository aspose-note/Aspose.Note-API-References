---
title: Image.Bytes
second_title: Aspose.Note untuk Referensi .NET API
description: Image Properti. Mendapatkan penyimpanan data gambar.
type: docs
weight: 50
url: /id/net/aspose.note/image/bytes/
---
## Image.Bytes property

Mendapatkan penyimpanan data gambar.

```csharp
public byte[] Bytes { get; }
```

### Contoh

Menunjukkan cara mendapatkan gambar dari dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dapatkan semua node Gambar
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Simpan byte gambar ke file
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### Lihat juga

* class [Image](../)
* ruang nama [Aspose.Note](../../image/)
* perakitan [Aspose.Note](../../../)


