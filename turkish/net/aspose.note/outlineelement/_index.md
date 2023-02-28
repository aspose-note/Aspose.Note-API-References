---
title: Class OutlineElement
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.OutlineElement sınıf. Bir OutlineElementı Temsil Eder.
type: docs
weight: 460
url: /tr/net/aspose.note/outlineelement/
---
## OutlineElement class

Bir OutlineElement'ı Temsil Eder.

```csharp
public sealed class OutlineElement : IndentatedNode<IOutlineElementChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [OutlineElement](outlineelement/#constructor)() | Yeni bir örneğini başlatır.`OutlineElement` sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [CreationTime](../../aspose.note/outlineelement/creationtime/) { get; set; } | Oluşturma zamanını alır veya ayarlar. |
| [Document](../../aspose.note/node/document/) { get; } | Düğümün belgesini alır. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/outlineelement/lastmodifiedtime/) { get; set; } | Son değiştirilme zamanını alır veya ayarlar. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Aynı düğüm ağacı seviyesindeki bir sonraki düğümü alır. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Düğüm türünü alır. |
| [NumberList](../../aspose.note/outlineelement/numberlist/) { get; set; } | Numaralı liste başlığının stilini alır veya ayarlar. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Üst düğümü alır. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Aynı düğüm ağacı seviyesindeki önceki düğümü alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Accept](../../aspose.note/outlineelement/accept/)(DocumentVisitor) | Düğümün ziyaretçisini kabul eder. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineElementChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineElementChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Örnekler

Etiketli yeni resmin nasıl ekleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Document sınıfından bir nesne oluşturun
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

// Ana hat öğesi düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

Listenin biçimlendirmesiyle ilgili bilgilerin nasıl alınacağını gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Anahat öğesinin toplama düğümlerini alın
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Her düğümü yinele
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Yazı tipi adını al
        Console.WriteLine("Font Name: " + list.Font);

        // yazı tipi uzunluğunu al
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Yazı tipi boyutunu al
        Console.WriteLine("Font Size: " + list.FontSize);

        // yazı tipi rengini al
        Console.WriteLine("Font Color: " + list.FontColor);

        // formatı al
        Console.WriteLine("Font format: " + list.Format);

        // kalın işaretle
        Console.WriteLine("Is bold: " + list.IsBold);

        // italik kontrol et
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

Çince numaralandırma ile yeni listenin nasıl ekleneceğini gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// OneNote belgesini başlat
Aspose.Note.Document doc = new Aspose.Note.Document();

// OneNote sayfasını başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Metin stili ayarlarını uygula
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Aynı çerçevedeki sayılar otomatik olarak artırılır.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Yeni madde işaretli listelerin nasıl ekleneceğini gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Document sınıfından bir nesne oluşturun
Aspose.Note.Document doc = new Aspose.Note.Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline sınıf nesnesini başlat
Outline outline = new Outline(doc);

// TextStyle sınıf nesnesini başlat ve biçimlendirme özelliklerini ayarla
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement sınıf nesnelerini başlat ve madde işaretlerini uygula
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// RichText sınıf nesnesini başlat ve metin stilini uygula
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Anahat öğeleri ekle
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Anahat düğümü ekle
page.AppendChildLast(outline);
// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Numaralandırma ile yeni listenin nasıl ekleneceğini gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Document sınıfından bir nesne oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline sınıf nesnesini başlat
Outline outline = new Outline(doc);

// TextStyle sınıf nesnesini başlat ve biçimlendirme özelliklerini ayarla
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement sınıf nesnelerini başlat ve numaralandırmayı uygula
// Aynı çerçevedeki sayılar otomatik olarak artırılır.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Anahat öğeleri ekle
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Ayrıca bakınız

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


