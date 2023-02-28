---
title: Image.Alignment
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Image संपत्त. संरेखण प्रप्त करत है य सेट करत है
type: docs
weight: 20
url: /hi/net/aspose.note/image/alignment/
---
## Image.Alignment property

संरेखण प्राप्त करता है या सेट करता है।

```csharp
public HorizontalAlignment Alignment { get; set; }
```

### उदाहरण

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

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* नाम स्थान [Aspose.Note](../../image/)
* सभा [Aspose.Note](../../../)


