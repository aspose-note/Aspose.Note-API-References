---
title: Image.Height
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Image संपत्त. ऊंचई प्रप्त य सेट करत है यह MS OneNote दस्तवेज़ में छव क वस्तवक ऊंचई है.
type: docs
weight: 90
url: /hi/net/aspose.note/image/height/
---
## Image.Height property

ऊंचाई प्राप्त या सेट करता है। यह MS OneNote दस्तावेज़ में छवि की वास्तविक ऊंचाई है.

```csharp
public float Height { get; set; }
```

### उदाहरण

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

### यह सभी देखें

* class [Image](../)
* नाम स्थान [Aspose.Note](../../image/)
* सभा [Aspose.Note](../../../)


