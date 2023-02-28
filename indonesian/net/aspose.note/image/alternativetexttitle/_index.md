---
title: Image.AlternativeTextTitle
second_title: Aspose.Note untuk Referensi .NET API
description: Image Properti. Mendapat atau menetapkan judul teks alternatif untuk gambar.
type: docs
weight: 40
url: /id/net/aspose.note/image/alternativetexttitle/
---
## Image.AlternativeTextTitle property

Mendapat atau menetapkan judul teks alternatif untuk gambar.

```csharp
public string AlternativeTextTitle { get; set; }
```

### Contoh

Menunjukkan cara menyetel deskripsi teks untuk gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

### Lihat juga

* class [Image](../)
* ruang nama [Aspose.Note](../../image/)
* perakitan [Aspose.Note](../../../)


