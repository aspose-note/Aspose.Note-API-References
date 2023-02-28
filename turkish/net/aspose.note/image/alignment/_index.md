---
title: Image.Alignment
second_title: Aspose.Note for .NET API Referansı
description: Image mülk. Hizalamayı alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.note/image/alignment/
---
## Image.Alignment property

Hizalamayı alır veya ayarlar.

```csharp
public HorizontalAlignment Alignment { get; set; }
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

Akıştan bir belgeye nasıl resim ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Document sınıfından bir nesne oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Resim adını, uzantısını ve akışını kullanarak ikinci resmi yükleyin.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Görüntü hizalamasını ayarla
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Dosyadan belgeye nasıl resim ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Document sınıfından bir nesne oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline sınıf nesnesini başlat ve ofset özelliklerini ayarla
Outline outline = new Outline(doc);

// OutlineElement sınıf nesnesini başlat
OutlineElement outlineElem = new OutlineElement(doc);

// Dosya yoluna göre bir resim yükleyin.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Görüntü hizalamasını ayarla
                              Alignment = HorizontalAlignment.Right
                          };

// Resim eklemek
outlineElem.AppendChildLast(image);

// Anahat öğeleri ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Ayrıca bakınız

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* ad alanı [Aspose.Note](../../image/)
* toplantı [Aspose.Note](../../../)


