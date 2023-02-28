---
title: Image.HyperlinkUrl
second_title: Aspose.Note untuk Referensi .NET API
description: Image Properti. Mendapatkan atau menyetel hyperlink yang terkait dengan gambar.
type: docs
weight: 110
url: /id/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

Mendapatkan atau menyetel hyperlink yang terkait dengan gambar.

```csharp
public string HyperlinkUrl { get; set; }
```

### Contoh

Menunjukkan cara mengikat hyperlink ke gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://gambar.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### Lihat juga

* class [Image](../)
* ruang nama [Aspose.Note](../../image/)
* perakitan [Aspose.Note](../../../)


