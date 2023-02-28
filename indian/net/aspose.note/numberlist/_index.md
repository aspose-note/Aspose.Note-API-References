---
title: Class NumberList
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.NumberList कक्ष. क्रमंकत य बुलेटेड सूच क प्रतनधत्व करत है
type: docs
weight: 440
url: /hi/net/aspose.note/numberlist/
---
## NumberList class

क्रमांकित या बुलेटेड सूची का प्रतिनिधित्व करता है।

```csharp
public class NumberList
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | का एक नया उदाहरण प्रारंभ करता है`NumberList`class. यह उदाहरण बुलेटेड सूची का प्रतिनिधित्व करता है। |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | का एक नया उदाहरण प्रारंभ करता है`NumberList` class. यह उदाहरण क्रमांकित सूची का प्रतिनिधित्व करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | फ़ॉन्ट का नाम प्राप्त या सेट करता है। |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | फ़ॉन्ट रंग प्राप्त या सेट करता है। |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | फ़ॉन्ट आकार प्राप्त या सेट करता है। |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | लाइन हेडर का प्रारूप प्राप्त या सेट करता है। बुलेटेड सूचियों के लिए बुलेट प्रतीक का प्रतिनिधित्व करता है। |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि टेक्स्ट शैली बोल्ड है या नहीं। |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | टेक्स्ट शैली इटैलिक है या नहीं, यह इंगित करने वाला मान प्राप्त या सेट करता है। |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | अंतिम संशोधित समय प्राप्त या सेट करता है। |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | स्वचालित रूप से क्रमांकित वस्तुओं के समूह के लिए उपयोग किए जाने वाले संख्या प्रारूप को प्राप्त या सेट करता है। बुलेटेड सूचियों के लिए शून्य होना चाहिए। |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | सूची आइटम के स्वचालित संख्या मान को ओवरराइड करने वाले संख्यात्मक मान को प्राप्त या सेट करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | निर्धारित करता है कि निर्दिष्ट वस्तु वर्तमान वस्तु के बराबर है या नहीं। |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | निर्धारित करता है कि निर्दिष्ट वस्तु वर्तमान वस्तु के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | प्रकार के लिए हैश फ़ंक्शन के रूप में कार्य करता है। |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | क्रमांकित सूची शीर्षलेख प्राप्त करता है। |

### उदाहरण

दिखाता है कि सूची के स्वरूपण के बारे में जानकारी कैसे प्राप्त करें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// रूपरेखा तत्व के संग्रह नोड्स को पुनः प्राप्त करें
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// प्रत्येक नोड के माध्यम से दोहराएं
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // फ़ॉन्ट नाम पुनर्प्राप्त करें
        Console.WriteLine("Font Name: " + list.Font);

        // फ़ॉन्ट लंबाई पुनर्प्राप्त करें
        Console.WriteLine("Font Length: " + list.Font.Length);

        // फ़ॉन्ट आकार पुनर्प्राप्त करें
        Console.WriteLine("Font Size: " + list.FontSize);

        // फ़ॉन्ट रंग पुनर्प्राप्त करें
        Console.WriteLine("Font Color: " + list.FontColor);

        // स्वरूप प्राप्त करें
        Console.WriteLine("Font format: " + list.Format);

        // बोल्ड चेक करें
        Console.WriteLine("Is bold: " + list.IsBold);

        // इटैलिक चेक करें
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
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

* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


