---
title: Class TextStyle
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.TextStyle कक्ष. पठ शैल नर्दष्ट करत है
type: docs
weight: 970
url: /hi/net/aspose.note/textstyle/
---
## TextStyle class

पाठ शैली निर्दिष्ट करता है।

```csharp
public sealed class TextStyle : Style
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TextStyle](textstyle/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | "एन-यूएस" संस्कृति के साथ शैली प्राप्त करता है। |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | एमएस वनोट में शीर्षक तिथि के लिए डिफ़ॉल्ट शैली प्राप्त करता है। |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | एमएस वनोट में शीर्षक पाठ के लिए डिफ़ॉल्ट शैली प्राप्त करता है। |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | एमएस वनोट में शीर्षक समय के लिए डिफ़ॉल्ट शैली प्राप्त करता है। |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | फ़ॉन्ट रंग प्राप्त या सेट करता है। |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | फ़ॉन्ट नाम प्राप्त या सेट करता है। |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | फ़ॉन्ट आकार प्राप्त या सेट करता है। |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | फ़ॉन्ट शैली प्राप्त करता है। |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | हाइलाइट रंग प्राप्त या सेट करता है। |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | हाइपरलिंक पता प्राप्त या सेट करता है। सेट किया जाना चाहिए यदि का मान[`IsHyperlink`](./ishyperlink/) संपत्ति सत्य है। |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि टेक्स्ट शैली बोल्ड है या नहीं। |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | टेक्स्ट शैली छिपी हुई है या नहीं यह इंगित करने वाला मान प्राप्त या सेट करता है। |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | टेक्स्ट शैली हाइपरलिंक है या नहीं यह इंगित करने वाला मान प्राप्त या सेट करता है। |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | टेक्स्ट शैली इटैलिक है या नहीं, यह इंगित करने वाला मान प्राप्त या सेट करता है। |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि पाठ शैली गणित-स्वरूपण है या नहीं। |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | एक मान प्राप्त या सेट करता है जो बताता है कि पाठ शैली स्ट्राइकथ्रू है या नहीं। |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि पाठ शैली सबस्क्रिप्ट है। |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि पाठ शैली सुपरस्क्रिप्ट है या नहीं। |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि पाठ शैली रेखांकित है या नहीं। |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | टेक्स्ट की भाषा प्राप्त या सेट करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | निर्धारित करता है कि निर्दिष्ट वस्तु वर्तमान वस्तु के बराबर है या नहीं। |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | निर्धारित करता है कि निर्दिष्ट वस्तु वर्तमान वस्तु के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | प्रकार के लिए हैश फ़ंक्शन के रूप में कार्य करता है। |

### उदाहरण

फ़ॉन्ट का आकार बढ़ाकर अन्य शीर्षकों के बीच पृष्ठ के शीर्षक पर जोर दें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Aspose.one");

// पृष्ठ के शीर्षकों के माध्यम से पुनरावृति करें।
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

हाइलाइट करके नवीनतम टेक्स्ट के परिवर्तनों पर जोर दें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document document = new Document(dataDir + "Aspose.one");

// RichText नोड्स को पिछले सप्ताह संशोधित करें।
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // हाइलाइट रंग सेट करें
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // हाइलाइट रंग सेट करें
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

टेक्स्ट के लिए अशुद्धि जाँच भाषा सेट करें।

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

अनुच्छेद शैली का उपयोग करके पाठ प्रारूप में हेरफेर करें।

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

दिखाता है कि हाइपरलिंक को टेक्स्ट से कैसे बाइंड किया जाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tasks();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
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

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem);

// टाइटल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Title title = new Title() { TitleText = titleText };

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Page page = new Note.Page() { Title = title };

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### यह सभी देखें

* class [Style](../style/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


