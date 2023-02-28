---
title: Class Image
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Image कक्ष. एक छव क प्रतनधत्व करत है
type: docs
weight: 250
url: /hi/net/aspose.note/image/
---
## Image class

एक छवि का प्रतिनिधित्व करता है।

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Image](image/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`Image` वर्ग. |
| [Image](image/#constructor_4)(string, Stream) | का एक नया उदाहरण प्रारंभ करता है`Image` वर्ग. |
| [Image](image/#constructor_5)(string, string, string) | का एक नया उदाहरण प्रारंभ करता है`Image` वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | संरेखण प्राप्त करता है या सेट करता है। |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | छवि के लिए एक वैकल्पिक टेक्स्ट प्राप्त करता है या सेट करता है। |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | छवि के लिए वैकल्पिक पाठ का शीर्षक प्राप्त या सेट करता है। |
| [Bytes](../../aspose.note/image/bytes/) { get; } | छवि डेटा स्टोर प्राप्त करता है। |
| [Document](../../aspose.note/node/document/) { get; } | नोड का दस्तावेज़ प्राप्त करता है। |
| [FileName](../../aspose.note/image/filename/) { get; } | फ़ाइल का नाम प्राप्त करता है। |
| [FilePath](../../aspose.note/image/filepath/) { get; } | छवि फ़ाइल का पथ प्राप्त करता है। |
| [Format](../../aspose.note/image/format/) { get; } | छवि का प्रारूप प्राप्त करता है। |
| [Height](../../aspose.note/image/height/) { get; set; } | ऊंचाई प्राप्त या सेट करता है। यह MS OneNote दस्तावेज़ में छवि की वास्तविक ऊंचाई है. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | क्षैतिज ऑफसेट प्राप्त या सेट करता है। |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | छवि से जुड़े हाइपरलिंक को प्राप्त या सेट करता है। |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | प्राप्त करता है कि छवि एक पृष्ठभूमि छवि है या नहीं। |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | एक मान प्राप्त करता है जो इंगित करता है कि यह नोड समग्र है या नहीं। यदि सही है तो नोड में चाइल्ड नोड हो सकते हैं. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | अंतिम संशोधित समय प्राप्त या सेट करता है। |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | उसी नोड ट्री स्तर पर अगला नोड प्राप्त करता है। |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | नोड प्रकार प्राप्त करता है। |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | मूल ऊंचाई प्राप्त करता है। आकार बदलने से पहले, यह छवि की मूल चौड़ाई है. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | मूल चौड़ाई प्राप्त करता है। आकार बदलने से पहले, यह छवि की मूल चौड़ाई है. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | मूल नोड प्राप्त करता है। |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | पिछले नोड को उसी नोड ट्री स्तर पर प्राप्त करता है। |
| [Tags](../../aspose.note/image/tags/) { get; } | अनुच्छेद के सभी टैग की सूची प्राप्त करता है। |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | वर्टिकल ऑफ़सेट प्राप्त या सेट करता है। |
| [Width](../../aspose.note/image/width/) { get; set; } | चौड़ाई प्राप्त या सेट करता है। यह MS OneNote दस्तावेज़ में छवि की वास्तविक चौड़ाई है. |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | नोड के आगंतुक को स्वीकार करता है। |

### उदाहरण

दिखाता है कि हाइपरलिंक को इमेज से कैसे बाइंड किया जाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

छवि के लिए टेक्स्ट विवरण सेट करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

दस्तावेज़ से छवि प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// सभी छवि नोड्स प्राप्त करें
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // इमेज बाइट्स को फाइल में सेव करें
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

छवि की मेटा जानकारी प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// सभी छवि नोड्स प्राप्त करें
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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

उपयोगकर्ता परिभाषित गुणों के साथ फ़ाइल से दस्तावेज़ में छवि जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// धारा से दस्तावेज़ लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

// दस्तावेज़ का पहला पृष्ठ प्राप्त करें।
Aspose.Note.Page page = doc.FirstChild;

// फ़ाइल से एक छवि लोड करें।
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // अपनी आवश्यकताओं के अनुसार छवि का आकार बदलें (वैकल्पिक)।
                              Width = 100,
                              Height = 100,

                              // पृष्ठ में छवि का स्थान सेट करें (वैकल्पिक)।
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // छवि संरेखण सेट करें
                              Alignment = HorizontalAlignment.Right
                          };

// छवि को पेज में जोड़ें।
page.AppendChildLast(image);
```

दिखाता है कि किसी छवि को स्ट्रीम से किसी दस्तावेज़ में कैसे जोड़ा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // छवि नाम, एक्सटेंशन और स्ट्रीम का उपयोग करके दूसरी छवि लोड करें।
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // छवि संरेखण सेट करें
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

फ़ाइल से दस्तावेज़ में छवि जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और ऑफ़सेट प्रॉपर्टी सेट करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);

// फ़ाइल पथ द्वारा एक छवि लोड करें।
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // छवि संरेखण सेट करें
                              Alignment = HorizontalAlignment.Right
                          };

// छवि जोड़ें
outlineElem.AppendChildLast(image);

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### यह सभी देखें

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


