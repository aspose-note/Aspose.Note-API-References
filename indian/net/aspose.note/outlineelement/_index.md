---
title: Class OutlineElement
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.OutlineElement कक्ष. एक रूपरेख तत्व क प्रतनधत्व करत है
type: docs
weight: 460
url: /hi/net/aspose.note/outlineelement/
---
## OutlineElement class

एक रूपरेखा तत्व का प्रतिनिधित्व करता है।

```csharp
public sealed class OutlineElement : IndentatedNode<IOutlineElementChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [OutlineElement](outlineelement/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`OutlineElement` वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| [CreationTime](../../aspose.note/outlineelement/creationtime/) { get; set; } | निर्माण समय प्राप्त या सेट करता है। |
| [Document](../../aspose.note/node/document/) { get; } | नोड का दस्तावेज़ प्राप्त करता है। |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/outlineelement/lastmodifiedtime/) { get; set; } | अंतिम संशोधित समय प्राप्त या सेट करता है। |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | उसी नोड ट्री स्तर पर अगला नोड प्राप्त करता है। |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | नोड प्रकार प्राप्त करता है। |
| [NumberList](../../aspose.note/outlineelement/numberlist/) { get; set; } | क्रमांकित सूची शीर्षलेख के लिए शैली प्राप्त या सेट करता है। |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | मूल नोड प्राप्त करता है। |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | पिछले नोड को उसी नोड ट्री स्तर पर प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [Accept](../../aspose.note/outlineelement/accept/)(DocumentVisitor) | नोड के आगंतुक को स्वीकार करता है। |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineElementChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineElementChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### उदाहरण

टैग के साथ नई छवि जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);

// छवि लोड करें
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// दस्तावेज़ नोड में छवि डालें
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// रूपरेखा तत्व नोड जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

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

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


