---
title: Image.Height
second_title: Aspose.Note for .NET API Referansı
description: Image mülk. Yüksekliği alır veya ayarlar. Bu MS OneNote belgesindeki görüntünün gerçek yüksekliğidir.
type: docs
weight: 90
url: /tr/net/aspose.note/image/height/
---
## Image.Height property

Yüksekliği alır veya ayarlar. Bu, MS OneNote belgesindeki görüntünün gerçek yüksekliğidir.

```csharp
public float Height { get; set; }
```

### Örnekler

Görüntünün meta bilgilerinin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm Görüntü düğümlerini al
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


