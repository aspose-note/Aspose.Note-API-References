---
title: Image
second_title: Aspose.Note for .NET API Referansı
description: Bir Görüntüyü Temsil Eder.
type: docs
weight: 240
url: /tr/net/aspose.note/image/
---
## Image class

Bir Görüntüyü Temsil Eder.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Image](image#constructor)() | Yeni bir örneğini başlatır[`Image`](../image) sınıf. |
| [Image](image#constructor_4)(string, Stream) | Yeni bir örneğini başlatır[`Image`](../image) sınıf. |
| [Image](image#constructor_5)(string, string, string) | Yeni bir örneğini başlatır[`Image`](../image) sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment) { get; set; } | Hizalamayı alır veya ayarlar. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription) { get; set; } | Resim için alternatif bir metin gövdesi alır veya ayarlar. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle) { get; set; } | Resim için alternatif bir metin başlığı alır veya ayarlar. |
| [Bytes](../../aspose.note/image/bytes) { get; } | Görüntü veri deposunu alır. |
| [Document](../../aspose.note/node/document) { get; } | Düğümün belgesini alır. |
| [FileName](../../aspose.note/image/filename) { get; } | Dosya adını alır. |
| [FilePath](../../aspose.note/image/filepath) { get; } | Görüntü dosyasının yolunu alır. |
| [Format](../../aspose.note/image/format) { get; } | Resmin biçimini alır. |
| [Height](../../aspose.note/image/height) { get; set; } | Yüksekliği alır veya ayarlar. Bu, MS OneNote belgesindeki görüntünün gerçek yüksekliğidir. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset) { get; set; } | Yatay ofseti alır veya ayarlar. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl) { get; set; } | Görüntüyle ilişkili köprüyü alır veya ayarlar. |
| [IsBackground](../../aspose.note/image/isbackground) { get; set; } | Resmin bir arka plan resmi olup olmadığını alır. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Bu düğümün bileşik olup olmadığını gösteren bir değer alır. Doğruysa, düğümün alt düğümleri olabilir. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime) { get; set; } | Son değiştirilme zamanını alır veya ayarlar. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Aynı düğüm ağacı düzeyinde bir sonraki düğümü alır. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Düğüm türünü alır. |
| [OriginalHeight](../../aspose.note/image/originalheight) { get; } | Orijinal yüksekliği alır. Bu, resmin yeniden boyutlandırmadan önceki orijinal genişliğidir. |
| [OriginalWidth](../../aspose.note/image/originalwidth) { get; } | Orijinal genişliği alır. Bu, resmin yeniden boyutlandırmadan önceki orijinal genişliğidir. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Üst düğümü alır. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Aynı düğüm ağacı düzeyinde önceki düğümü alır. |
| [Tags](../../aspose.note/image/tags) { get; } | Bir paragrafın tüm etiketlerinin listesini alır. |
| [VerticalOffset](../../aspose.note/image/verticaloffset) { get; set; } | Dikey ofseti alır veya ayarlar. |
| [Width](../../aspose.note/image/width) { get; set; } | Genişliği alır veya ayarlar. Bu, MS OneNote belgesindeki görüntünün gerçek genişliğidir. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Accept](../../aspose.note/image/accept)(DocumentVisitor) | Düğümün ziyaretçisini kabul eder. |

### Örnekler

Bir görüntüye bir köprünün nasıl bağlanacağını gösterir.

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

Bir görüntü için metin açıklamasının nasıl ayarlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
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

Bir belgeden nasıl görüntü alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm Görüntü düğümlerini al
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Görüntü baytlarını bir dosyaya kaydet
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Resmin meta bilgilerinin nasıl alınacağını gösterir.

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

Etiketli yeni resmin nasıl ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline sınıf nesnesini başlat
Outline outline = new Outline(doc);

// OutlineElement sınıf nesnesini başlat
OutlineElement outlineElem = new OutlineElement(doc);

// Bir resim yükle
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Belge düğümüne resim ekle
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Anahat öğesi düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

Kullanıcı tanımlı özelliklere sahip bir belgeye dosyadan nasıl resim ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Images();

// Akıştan belge yükle.
Document doc = new Document(dataDir + "Aspose.one");

// Belgenin ilk sayfasını al.
Aspose.Note.Page page = doc.FirstChild;

// Dosyadan bir resim yükleyin.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Resmin boyutunu ihtiyaçlarınıza göre değiştirin (isteğe bağlı).
                              Width = 100,
                              Height = 100,

                              // Resmin sayfadaki konumunu ayarlayın (isteğe bağlı).
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

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Görüntü adını, uzantısını ve akışını kullanarak ikinci görüntüyü yükleyin.
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

// Document sınıfının bir nesnesini oluşturun
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

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* ad alanı [Aspose.Note](../../aspose.note)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
