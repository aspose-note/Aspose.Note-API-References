---
title: Image.Height
second_title: Aspose.Note untuk Referensi .NET API
description: Image Properti. Mendapat atau mengatur ketinggian. Ini adalah tinggi sebenarnya dari gambar di dokumen MS OneNote.
type: docs
weight: 90
url: /id/net/aspose.note/image/height/
---
## Image.Height property

Mendapat atau mengatur ketinggian. Ini adalah tinggi sebenarnya dari gambar di dokumen MS OneNote.

```csharp
public float Height { get; set; }
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

Menunjukkan cara menambahkan gambar dari file ke dokumen dengan properti yang ditentukan pengguna.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Muat dokumen dari aliran.
Document doc = new Document(dataDir + "Aspose.one");

// Dapatkan halaman pertama dokumen.
Aspose.Note.Page page = doc.FirstChild;

// Memuat gambar dari file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ubah ukuran gambar sesuai kebutuhan Anda (opsional).
                              Width = 100,
                              Height = 100,

                              // Tetapkan lokasi gambar di halaman (opsional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Atur perataan gambar
                              Alignment = HorizontalAlignment.Right
                          };

// Tambahkan gambar ke halaman.
page.AppendChildLast(image);
```

### Lihat juga

* class [Image](../)
* ruang nama [Aspose.Note](../../image/)
* perakitan [Aspose.Note](../../../)


