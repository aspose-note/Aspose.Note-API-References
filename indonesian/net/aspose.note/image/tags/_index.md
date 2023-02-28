---
title: Image.Tags
second_title: Aspose.Note untuk Referensi .NET API
description: Image Properti. Mendapat daftar semua tag paragraf.
type: docs
weight: 160
url: /id/net/aspose.note/image/tags/
---
## Image.Tags property

Mendapat daftar semua tag paragraf.

```csharp
public List<ITag> Tags { get; }
```

### Contoh

Menunjukkan cara menambahkan gambar baru dengan tag.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Buat objek dari kelas Dokumen
Document doc = new Document();

// Inisialisasi objek kelas Halaman
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inisialisasi objek kelas Outline
Outline outline = new Outline(doc);

// Menginisialisasi objek kelas OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Memuat gambar
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Sisipkan gambar di simpul dokumen
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Tambahkan simpul elemen kerangka
outline.AppendChildLast(outlineElem);

// Tambahkan simpul kerangka
page.AppendChildLast(outline);

// Tambahkan simpul halaman
doc.AppendChildLast(page);

// Simpan dokumen OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### Lihat juga

* interface [ITag](../../itag/)
* class [Image](../)
* ruang nama [Aspose.Note](../../image/)
* perakitan [Aspose.Note](../../../)


