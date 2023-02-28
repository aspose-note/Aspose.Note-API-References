---
title: Style.FontName
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Style संपत्त. फ़न्ट नम प्रप्त य सेट करत है
type: docs
weight: 20
url: /hi/net/aspose.note/style/fontname/
---
## Style.FontName property

फ़ॉन्ट नाम प्राप्त या सेट करता है।

```csharp
public string FontName { get; set; }
```

### उदाहरण

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

* class [Style](../)
* नाम स्थान [Aspose.Note](../../style/)
* सभा [Aspose.Note](../../../)


