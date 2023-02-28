---
title: Image.VerticalOffset
second_title: Aspose.Note untuk Referensi .NET API
description: Image Properti. Mendapat atau menyetel offset vertikal.
type: docs
weight: 170
url: /id/net/aspose.note/image/verticaloffset/
---
## Image.VerticalOffset property

Mendapat atau menyetel offset vertikal.

```csharp
public float VerticalOffset { get; set; }
```

### Contoh

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


