---
title: CompositeNode1.GetChildNodes
second_title: Aspose.Note .NET API संदर्भ के लिए
description: CompositeNode तरक. नड प्रकर द्वर सभ चइल्ड नड प्रप्त करें.
type: docs
weight: 70
url: /hi/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

नोड प्रकार द्वारा सभी चाइल्ड नोड प्राप्त करें.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| पैरामीटर | विवरण |
| --- | --- |
| T1 | लौटाई गई सूची में तत्वों का प्रकार। |

### प्रतिलाभ की मात्रा

चाइल्ड नोड्स की सूची।

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

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* नाम स्थान [Aspose.Note](../../compositenode-1/)
* सभा [Aspose.Note](../../../)


