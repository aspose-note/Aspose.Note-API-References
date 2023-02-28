---
title: Image.Alignment
second_title: Aspose.Note untuk Referensi .NET API
description: Image Properti. Mendapat atau menyetel perataan.
type: docs
weight: 20
url: /id/net/aspose.note/image/alignment/
---
## Image.Alignment property

Mendapat atau menyetel perataan.

```csharp
public HorizontalAlignment Alignment { get; set; }
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

Menunjukkan cara menambahkan gambar dari aliran ke dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Muat gambar kedua menggunakan nama gambar, ekstensi, dan aliran.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Atur perataan gambar
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Menunjukkan cara menambahkan gambar dari file ke dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas Outline dan atur properti offset
Outline outline = new Outline(doc);

// Menginisialisasi objek kelas OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Muat gambar dengan jalur file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Atur perataan gambar
                              Alignment = HorizontalAlignment.Right
                          };

// Menambahkan gambar
outlineElem.AppendChildLast(image);

// Tambahkan elemen kerangka
outline.AppendChildLast(outlineElem);

// Tambahkan simpul Outline
page.AppendChildLast(outline);

// Tambahkan simpul Halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Lihat juga

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* ruang nama [Aspose.Note](../../image/)
* perakitan [Aspose.Note](../../../)


