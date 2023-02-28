---
title: Class ParagraphStyle
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.ParagraphStyle कक्ष. टेक्स्ट स्टइल सेटंग्स क उपयग कय जन चहए यद कई मेल खने वल टेक्स्ट स्टइल ऑब्जेक्ट नहं हैStyles संग्रह य त यह ऑब्जेक्ट आवश्यक सेटंग नर्दष्ट नहं करत है.
type: docs
weight: 510
url: /hi/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

टेक्स्ट स्टाइल सेटिंग्स का उपयोग किया जाना चाहिए, यदि कोई मेल खाने वाला टेक्स्ट स्टाइल ऑब्जेक्ट नहीं हैStyles संग्रह या तो यह ऑब्जेक्ट आवश्यक सेटिंग निर्दिष्ट नहीं करता है.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | का एक नया उदाहरण प्रारंभ करता है`ParagraphStyle` वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | डिफ़ॉल्ट सेटिंग्स के साथ ParagraphStyle प्राप्त करता है। |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | फ़ॉन्ट रंग प्राप्त या सेट करता है। |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | फ़ॉन्ट नाम प्राप्त या सेट करता है। |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | फ़ॉन्ट आकार प्राप्त या सेट करता है। |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | फ़ॉन्ट शैली प्राप्त करता है। |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | हाइलाइट रंग प्राप्त या सेट करता है। |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि टेक्स्ट शैली बोल्ड है या नहीं। |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | टेक्स्ट शैली इटैलिक है या नहीं, यह इंगित करने वाला मान प्राप्त या सेट करता है। |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | एक मान प्राप्त या सेट करता है जो बताता है कि पाठ शैली स्ट्राइकथ्रू है या नहीं। |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि पाठ शैली सबस्क्रिप्ट है। |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि पाठ शैली सुपरस्क्रिप्ट है या नहीं। |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो इंगित करता है कि पाठ शैली रेखांकित है या नहीं। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | निर्धारित करता है कि निर्दिष्ट वस्तु वर्तमान वस्तु के बराबर है या नहीं। |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | निर्धारित करता है कि निर्दिष्ट वस्तु वर्तमान वस्तु के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | प्रकार के लिए हैश फ़ंक्शन के रूप में कार्य करता है। |

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

दिखाता है कि चीनी क्रमांकन के साथ नई सूची कैसे सम्मिलित करें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// OneNote दस्तावेज़ को प्रारंभ करें
Aspose.Note.Document doc = new Aspose.Note.Document();

// OneNote पेज को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// टेक्स्ट स्टाइल सेटिंग लागू करें
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// एक ही रूपरेखा में संख्याएँ स्वतः बढ़ जाती हैं।
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//---------------------------------------------------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//---------------------------------------------------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//---------------------------------------------------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

दिखाता है कि नई बुलेटेड लिस कैसे डालें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Aspose.Note.Document doc = new Aspose.Note.Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// टेक्स्ट स्टाइल क्लास ऑब्जेक्ट प्रारंभ करें और स्वरूपण गुण सेट करें
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// OutlineElement क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और बुलेट्स अप्लाई करें
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// RichText क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और टेक्स्ट स्टाइल लागू करें
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);
// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

नंबरिंग के साथ नई सूची डालने का तरीका दिखाता है।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// टेक्स्ट स्टाइल क्लास ऑब्जेक्ट प्रारंभ करें और स्वरूपण गुण सेट करें
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट्स को इनिशियलाइज़ करें और नंबरिंग लागू करें
// एक ही रूपरेखा में संख्याएँ स्वतः बढ़ जाती हैं।
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### यह सभी देखें

* class [Style](../style/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


