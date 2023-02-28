---
title: Image.Bytes
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Image संपत्त. छव डेट स्टर प्रप्त करत है
type: docs
weight: 50
url: /hi/net/aspose.note/image/bytes/
---
## Image.Bytes property

छवि डेटा स्टोर प्राप्त करता है।

```csharp
public byte[] Bytes { get; }
```

### उदाहरण

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

### यह सभी देखें

* class [Image](../)
* नाम स्थान [Aspose.Note](../../image/)
* सभा [Aspose.Note](../../../)


