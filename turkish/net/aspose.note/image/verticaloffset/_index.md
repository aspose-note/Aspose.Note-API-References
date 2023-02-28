---
title: Image.VerticalOffset
second_title: Aspose.Note for .NET API Referansı
description: Image mülk. Dikey ofseti alır veya ayarlar.
type: docs
weight: 170
url: /tr/net/aspose.note/image/verticaloffset/
---
## Image.VerticalOffset property

Dikey ofseti alır veya ayarlar.

```csharp
public float VerticalOffset { get; set; }
```

### Örnekler

Kullanıcı tanımlı özelliklere sahip bir belgeye dosyadan nasıl resim ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Belgeyi akıştan yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

// Belgenin ilk sayfasını alın.
Aspose.Note.Page page = doc.FirstChild;

// Dosyadan bir resim yükleyin.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Görüntünün boyutunu ihtiyaçlarınıza göre değiştirin (isteğe bağlı).
                              Width = 100,
                              Height = 100,

                              // Görüntünün sayfadaki konumunu ayarlayın (isteğe bağlı).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Görüntü hizalamasını ayarla
                              Alignment = HorizontalAlignment.Right
                          };

// Resmi sayfaya ekleyin.
page.AppendChildLast(image);
```

### Ayrıca bakınız

* class [Image](../)
* ad alanı [Aspose.Note](../../image/)
* toplantı [Aspose.Note](../../../)


