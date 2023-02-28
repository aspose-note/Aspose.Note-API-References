---
title: Class RichText
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.RichText sınıf. Zengin bir metni temsil eder.
type: docs
weight: 530
url: /tr/net/aspose.note/richtext/
---
## RichText class

Zengin bir metni temsil eder.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [RichText](richtext/#constructor)() | Yeni bir örneğini başlatır.`RichText` sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | Hizalamayı alır veya ayarlar. |
| [Document](../../aspose.note/node/document/) { get; } | Düğümün belgesini alır. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Bu düğümün bileşik olup olmadığını gösteren bir değer alır. Doğruysa, düğümün alt düğümleri olabilir. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | Son değiştirilme zamanını alır veya ayarlar. |
| [Length](../../aspose.note/richtext/length/) { get; } | Metnin uzunluğunu alır. |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | Satır aralığını alır veya ayarlar. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Aynı düğüm ağacı seviyesindeki bir sonraki düğümü alır. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Düğüm türünü alır. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | Paragraf stilini alır veya ayarlar. Bu ayarlar, içinde eşleşen bir TextStyle nesnesi yoksa kullanılır.Styles koleksiyon ya bu nesne gerekli bir ayarı belirtmiyor. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Üst düğümü alır. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Aynı düğüm ağacı seviyesindeki önceki düğümü alır. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | . sonrasındaki minimum alan miktarını alır veya ayarlar. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | Önceki minimum alan miktarını alır veya ayarlar. |
| [Tags](../../aspose.note/richtext/tags/) { get; } | Bir paragrafın tüm etiketlerinin listesini alır. |
| [Text](../../aspose.note/richtext/text/) { get; set; } | Metni alır veya ayarlar. Dize, 10 (satır besleme). değerinde herhangi bir karakter İÇERMEZ OLMALIDIR |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | Metin çalıştırmalarının koleksiyonunu alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | Düğümün ziyaretçisini kabul eder. |
| [Append](../../aspose.note/richtext/append/#append)(string) | Son metin aralığına bir dize ekler. |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | Sonuna bir dize ekler. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | İlk metin aralığının önüne bir dize ekler. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | Öne bir dize ekler. |
| [Clear](../../aspose.note/richtext/clear/)() | Bu örneğin içeriğini temizler. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | Bu RichText nesnesinin karakterlerini yineleyen bir numaralandırıcı döndürür. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | Bu dizgede belirtilen Unicode karakterinin ilk geçtiği yerin sıfır tabanlı dizinini döndürür. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | Bu örnekte belirtilen dizenin ilk geçtiği yerin sıfır tabanlı dizinini döndürür. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | Bu dizgede belirtilen Unicode karakterinin ilk geçtiği yerin sıfır tabanlı dizinini döndürür. Arama belirtilen karakter konumunda başlar. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | Bu örnekte belirtilen dizenin ilk geçtiği yerin sıfır tabanlı dizinini döndürür. Arama belirtilen karakter konumunda başlar. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | Geçerli örnekte belirtilen dizenin ilk geçtiği yerin sıfır tabanlı dizinini döndürür. Bir parametre, belirtilen dize için kullanılacak arama türünü belirtir. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | Bu örnekte belirtilen karakterin ilk geçtiği yerin sıfır tabanlı dizinini döndürür. Arama belirli bir karakter konumunda başlar ve belirtilen sayıda karakter konumunu inceler. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | Bu örnekte belirtilen dizenin ilk geçtiği yerin sıfır tabanlı dizinini döndürür. Arama belirli bir karakter konumunda başlar ve belirtilen sayıda karakter konumunu inceler. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | Geçerli örnekte belirtilen dizenin ilk geçtiği yerin sıfır tabanlı dizinini döndürür. Parametreler, geçerli dizide başlangıç arama konumunu ve belirtilen dizi için kullanılacak arama türünü belirtir. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | Geçerli örnekte belirtilen dizenin ilk geçtiği yerin sıfır tabanlı dizinini döndürür. |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | Belirtilen dizini bu örnekte belirtilen dizin konumuna ekler. |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | Bu örnekte belirtilen dizin konumuna belirtilen stilde belirtilen bir dize ekler. |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | Belirli bir konumdan başlayıp son konuma kadar devam ederek geçerli örnekteki tüm karakterleri kaldırır. |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | Belirli bir konumdan başlayarak geçerli örnekte belirtilen sayıda karakteri kaldırır. |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | Belirtilen bir Unicode karakterinin bu örnekteki tüm oluşumlarını belirtilen başka bir Unicode karakteriyle değiştirir. |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | Geçerli örnekte belirtilen bir dizenin tüm oluşumlarını belirtilen başka bir dizeyle değiştirir. |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | Geçerli örnekte belirtilen bir dizenin tüm oluşumlarını belirtilen stilde belirtilen başka bir dizeyle değiştirir. |
| [Trim](../../aspose.note/richtext/trim/#trim)() | Baştaki ve sondaki tüm boşluk karakterlerini kaldırır. |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | Bir karakterin tüm baştaki ve sondaki örneklerini kaldırır. |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | Bir dizide belirtilen bir dizi karakterin tüm baştaki ve sondaki oluşumlarını kaldırır. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | Sondaki tüm boşluk karakterlerini kaldırır. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | Bir karakterin sonundaki tüm oluşumlarını kaldırır. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | Bir dizide belirtilen bir dizi karakterin sonundaki tüm oluşumlarını kaldırır. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | Öndeki tüm boşluk karakterlerini kaldırır. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | Belirli bir karakterin başta gelen tüm oluşumlarını kaldırır. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | Bir dizide belirtilen bir dizi karakterin başta gelen tüm oluşumlarını kaldırır. |

### Örnekler

Tüm metnin belgeden nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Metni al
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Çıktı ekranındaki metni yazdır
Console.WriteLine(text);
```

Sayfadaki tüm metnin nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Sayfa düğümlerinin listesini al
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Metni al
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Çıktı ekranındaki metni yazdır
    Console.WriteLine(text);
}
```

Font boyutunu büyüterek sayfa başlıklarını diğer başlıklar arasında öne çıkaralım.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document document = new Document(dataDir + "Aspose.one");

// Sayfa başlıklarını yineleyin.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

Her tablo satırından nasıl metin alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tables();

// Belgeyi Aspose.Note'a yükleyin.
Document document = new Document(dataDir + "Sample1.one");

// tablo düğümlerinin bir listesini al
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Tablo satırlarını yinele
    foreach (TableRow row in table)
    {
        // Metni al
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Çıktı ekranındaki metni yazdır
        Console.WriteLine(text);
    }
}
```

Bir tablodan nasıl metin alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tables();

// Belgeyi Aspose.Note'a yükleyin.
Document document = new Document(dataDir + "Sample1.one");

// tablo düğümlerinin bir listesini al
IList<Table> nodes = document.GetChildNodes<Table>();

// Tablo sayısını ayarla
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Metni al
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Çıktı ekranındaki metni yazdır
    Console.WriteLine(text);
}
```

En son metin değişikliklerini vurgulayarak vurgulayalım.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Belgeyi Aspose.Note'a yükleyin.
Document document = new Document(dataDir + "Aspose.one");

// RichText düğümlerinin geçen hafta değiştirilmesini sağlayın.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Vurgu rengini ayarla
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Vurgu rengini ayarla
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Bir sayfa için bir başlığın nasıl ayarlanacağını gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

Bir metin için yazım denetleme dilini ayarlayın.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

Tüm sayfaların nasıl geçileceğini ve metinde nasıl değiştirileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tüm RichText düğümlerini al
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Bir şeklin metnini değiştir
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Desteklenen herhangi bir dosya biçiminde kaydedin
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Paragraf stilini kullanarak metin biçimine göre işleyin.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

Bir tablonun hücrelerinden nasıl metin alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tables();

// Belgeyi Aspose.Note'a yükleyin.
Document document = new Document(dataDir + "Sample1.one");

// tablo düğümlerinin bir listesini al
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Tablo satırlarını yinele
    foreach (TableRow row in table)
    {
        // TableCell düğümlerinin listesini al
        // Tablo hücrelerini yinele
        foreach (TableCell cell in row)
        {
            // Metni al
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Çıktı ekranındaki metni yazdır
            Console.WriteLine(text);
        }
    }
}
```

Sayfa metninin nasıl geçileceğini ve değiştirileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Tüm RichText düğümlerini al
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Bir şeklin metnini değiştir
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Desteklenen herhangi bir dosya biçiminde kaydedin
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Bir belgenin nasıl oluşturulacağını ve varsayılan seçenekleri kullanarak html formatında kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote belgesini başlat
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Belgedeki tüm metin için varsayılan stil.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// HTML formatında kaydet
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Etiketli yeni paragrafın nasıl ekleneceğini gösterir.

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
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// Metin düğümü ekle
outlineElem.AppendChildLast(text);

// Ana hat öğesi düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

Bir belgenin nasıl oluşturulacağını ve belirtilen sayfa aralığında html formatında kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote belgesini başlat
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Belgedeki tüm metin için varsayılan stil.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML formatında kaydet
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Bir etiketin ayrıntılarına nasıl erişileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "TagFile.one");

// Tüm RichText düğümlerini al
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Her düğümü yinele
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // özellikleri al
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

Metin içeren bir belgenin nasıl oluşturulacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Document sınıfından bir nesne oluşturun
Document doc = new Document();

// Sayfa sınıfı nesnesini başlat
Page page = new Page(doc);

// Outline sınıf nesnesini başlat
Outline outline = new Outline(doc);

// OutlineElement sınıf nesnesini başlat
OutlineElement outlineElem = new OutlineElement(doc);

// TextStyle sınıf nesnesini başlat ve biçimlendirme özelliklerini ayarla
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// RichText sınıf nesnesini başlat ve metin stilini uygula
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// RichText düğümü ekle
outlineElem.AppendChildLast(text);

// OutlineElement düğümü ekle
outline.AppendChildLast(outlineElem);

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
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

Haftalık toplantı için bir şablonun nasıl hazırlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tags();

// Document sınıfından bir nesne oluşturun
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
```

Bir metne köprünün nasıl bağlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_Tasks();

// Document sınıfından bir nesne oluşturun
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Anahat öğeleri ekle
outline.AppendChildLast(outlineElem);

// Başlık sınıfı nesnesini başlat
Title title = new Title() { TitleText = titleText };

// Sayfa sınıfı nesnesini başlat
Page page = new Note.Page() { Title = title };

// Anahat düğümü ekle
page.AppendChildLast(outline);

// Sayfa düğümü ekle
doc.AppendChildLast(page);

// OneNote belgesini kaydet
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Ayrıca bakınız

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


