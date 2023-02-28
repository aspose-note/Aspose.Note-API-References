---
title: Image.LastModifiedTime
second_title: Aspose.Note untuk Referensi .NET API
description: Image Properti. Mendapatkan atau menetapkan waktu modifikasi terakhir.
type: docs
weight: 130
url: /id/net/aspose.note/image/lastmodifiedtime/
---
## Image.LastModifiedTime property

Mendapatkan atau menetapkan waktu modifikasi terakhir.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Contoh

Menunjukkan cara mendapatkan informasi meta gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dapatkan semua node Gambar
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

### Lihat juga

* class [Image](../)
* ruang nama [Aspose.Note](../../image/)
* perakitan [Aspose.Note](../../../)


