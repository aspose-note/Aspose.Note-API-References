---
title: Class TextStyle
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.TextStyle sınıf. Metin stilini belirtir.
type: docs
weight: 970
url: /tr/net/aspose.note/textstyle/
---
## TextStyle class

Metin stilini belirtir.

```csharp
public sealed class TextStyle : Style
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [TextStyle](textstyle/)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | "en-US" kültürüne sahip stili alır. |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | MS OneNote'ta başlık tarihi için varsayılan stili alır. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | MS OneNote'ta başlık metni için varsayılan stili alır. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | MS OneNote'ta başlık zamanı için varsayılan stili alır. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Yazı tipi rengini alır veya ayarlar. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Yazı tipi adını alır veya ayarlar. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Yazı tipi boyutunu alır veya ayarlar. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Yazı tipi stilini alır. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Vurgu rengini alır veya ayarlar. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | Köprü adresini alır veya ayarlar. değeri ise ayarlanmalıdır.[`IsHyperlink`](./ishyperlink/) özellik true. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Metin stilinin kalın olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | Metin stilinin gizli olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | Metin stilinin köprü olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Metin stilinin italik olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | Metin stilinin matematik biçimlendirme olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Metin stilinin üstü çizili olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Metin stilinin alt simge olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Metin stilinin üst simge olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Metin stilinin altı çizili olup olmadığını gösteren bir değer alır veya ayarlar. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | Metnin dilini alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | Belirtilen nesnenin geçerli nesneye eşit olup olmadığını belirler. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | Belirtilen nesnenin geçerli nesneye eşit olup olmadığını belirler. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | type. için bir hash işlevi olarak hizmet eder |

### Örnekler

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

* class [Style](../style/)
* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


