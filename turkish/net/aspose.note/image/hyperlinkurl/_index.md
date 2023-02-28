---
title: Image.HyperlinkUrl
second_title: Aspose.Note for .NET API Referansı
description: Image mülk. Görüntüyle ilişkili köprüyü alır veya ayarlar.
type: docs
weight: 110
url: /tr/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

Görüntüyle ilişkili köprüyü alır veya ayarlar.

```csharp
public string HyperlinkUrl { get; set; }
```

### Örnekler

Bir görüntüye köprünün nasıl bağlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://resim.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### Ayrıca bakınız

* class [Image](../)
* ad alanı [Aspose.Note](../../image/)
* toplantı [Aspose.Note](../../../)


