---
title: NumberList
second_title: Aspose.Note for .NET API Referansı
description: Numaralı veya madde işaretli listeyi temsil eder.
type: docs
weight: 420
url: /tr/net/aspose.note/numberlist/
---
## NumberList class

Numaralı veya madde işaretli listeyi temsil eder.

```csharp
public class NumberList
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [NumberList](numberlist#constructor_1)(string, string, int) | Yeni bir örneğini başlatır[`NumberList`](../numberlist) class. Bu örnek madde işaretli bir listeyi temsil ediyor. |
| [NumberList](numberlist#constructor)(string, NumberFormat, string, int) | Yeni bir örneğini başlatır[`NumberList`](../numberlist)class. Bu örnek numaralı bir listeyi temsil ediyor. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Font](../../aspose.note/numberlist/font) { get; set; } | Yazı tipinin adını alır veya ayarlar. |
| [FontColor](../../aspose.note/numberlist/fontcolor) { get; set; } | Yazı tipi rengini alır veya ayarlar. |
| [FontSize](../../aspose.note/numberlist/fontsize) { get; set; } | Yazı tipi boyutunu alır veya ayarlar. |
| [Format](../../aspose.note/numberlist/format) { get; set; } | Satır başlığının biçimini alır veya ayarlar. Madde işaretli listeler için bir madde işareti sembolünü temsil eder. |
| [IsBold](../../aspose.note/numberlist/isbold) { get; set; } | Metin stilinin kalın olup olmadığını belirten bir değer alır veya ayarlar. |
| [IsItalic](../../aspose.note/numberlist/isitalic) { get; set; } | Metin stilinin italik olup olmadığını belirten bir değer alır veya ayarlar. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime) { get; set; } | Son değiştirilme zamanını alır veya ayarlar. |
| [NumberFormat](../../aspose.note/numberlist/numberformat) { get; set; } | Otomatik olarak numaralandırılmış bir grup nesne için kullanılan sayı biçimini alır veya ayarlar. Madde işaretli listeler için null olmalıdır. |
| [Restart](../../aspose.note/numberlist/restart) { get; set; } | Liste öğesinin otomatik sayı değerini geçersiz kılan sayısal değeri alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals#equals)(NumberList) | Belirtilen nesnenin geçerli nesneye eşit olup olmadığını belirler. |
| override [Equals](../../aspose.note/numberlist/equals#equals_1)(object) | Belirtilen nesnenin geçerli nesneye eşit olup olmadığını belirler. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode)() | type. için bir karma işlevi olarak hizmet eder |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader)(int) | Numaralandırılmış liste başlığını alır. |

### Örnekler

Listenin biçimlendirmesiyle ilgili bilgilerin nasıl alınacağını gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Anahat öğesinin bir koleksiyon düğümünü alın
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Her düğümde yineleme
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Yazı tipi adını al
        Console.WriteLine("Font Name: " + list.Font);

        // Yazı tipi uzunluğunu al
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Yazı tipi boyutunu al
        Console.WriteLine("Font Size: " + list.FontSize);

        // Yazı tipi rengini al
        Console.WriteLine("Font Color: " + list.FontColor);

        // Biçimi al
        Console.WriteLine("Font format: " + list.Format);

        // Kalınlığı kontrol et
        Console.WriteLine("Is bold: " + list.IsBold);

        // italik kontrol edin
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

// Aynı anahattaki sayılar otomatik olarak artırılır.
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

Numaralandırma ile yeni listenin nasıl ekleneceğini gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Document sınıfının bir nesnesini oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline sınıf nesnesini başlat
Outline outline = new Outline(doc);

// TextStyle sınıf nesnesini başlat ve biçimlendirme özelliklerini ayarla
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement sınıf nesnelerini başlat ve numaralandırma uygula
// Aynı anahattaki sayılar otomatik olarak artırılır.
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

* ad alanı [Aspose.Note](../../aspose.note)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
