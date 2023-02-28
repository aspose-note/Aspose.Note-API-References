---
title: CompositeNode1.GetChildNodes
second_title: Aspose.Note untuk Referensi .NET API
description: CompositeNode metode. Dapatkan semua simpul anak berdasarkan jenis simpul.
type: docs
weight: 70
url: /id/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

Dapatkan semua simpul anak berdasarkan jenis simpul.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parameter | Keterangan |
| --- | --- |
| T1 | Jenis elemen dalam daftar yang dikembalikan. |

### Nilai Pengembalian

Daftar node anak.

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

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* ruang nama [Aspose.Note](../../compositenode-1/)
* perakitan [Aspose.Note](../../../)


