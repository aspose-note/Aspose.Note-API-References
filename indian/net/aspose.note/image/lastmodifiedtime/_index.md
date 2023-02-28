---
title: Image.LastModifiedTime
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Image संपत्त. अंतम संशधत समय प्रप्त य सेट करत है
type: docs
weight: 130
url: /hi/net/aspose.note/image/lastmodifiedtime/
---
## Image.LastModifiedTime property

अंतिम संशोधित समय प्राप्त या सेट करता है।

```csharp
public DateTime LastModifiedTime { get; set; }
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


