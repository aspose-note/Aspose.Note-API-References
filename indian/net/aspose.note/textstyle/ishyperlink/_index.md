---
title: TextStyle.IsHyperlink
second_title: Aspose.Note .NET API संदर्भ के लिए
description: TextStyle संपत्त. टेक्स्ट शैल हइपरलंक है य नहं यह इंगत करने वल मन प्रप्त य सेट करत है
type: docs
weight: 80
url: /hi/net/aspose.note/textstyle/ishyperlink/
---
## TextStyle.IsHyperlink property

टेक्स्ट शैली हाइपरलिंक है या नहीं यह इंगित करने वाला मान प्राप्त या सेट करता है।

```csharp
public bool IsHyperlink { get; set; }
```

### उदाहरण

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

* class [TextStyle](../)
* नाम स्थान [Aspose.Note](../../textstyle/)
* सभा [Aspose.Note](../../../)


