---
title: Image.OriginalHeight
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Image संपत्त. मूल ऊंचई प्रप्त करत है आकर बदलने से पहले यह छव क मूल चड़ई है.
type: docs
weight: 140
url: /hi/net/aspose.note/image/originalheight/
---
## Image.OriginalHeight property

मूल ऊंचाई प्राप्त करता है। आकार बदलने से पहले, यह छवि की मूल चौड़ाई है.

```csharp
public float OriginalHeight { get; }
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

### यह सभी देखें

* class [Image](../)
* नाम स्थान [Aspose.Note](../../image/)
* सभा [Aspose.Note](../../../)


