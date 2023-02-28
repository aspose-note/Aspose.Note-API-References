---
title: AttachedFile.Bytes
second_title: Aspose.Note .NET API संदर्भ के लिए
description: AttachedFile संपत्त. एम्बेडेड फ़इल के लए बइनर डेट प्रप्त करत है
type: docs
weight: 50
url: /hi/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

एम्बेडेड फ़ाइल के लिए बाइनरी डेटा प्राप्त करता है।

```csharp
public byte[] Bytes { get; }
```

### उदाहरण

संलग्न फ़ाइल की सामग्री प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Attachments();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Sample1.one");

// संलग्न फ़ाइल नोड्स की सूची प्राप्त करें
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// सभी नोड्स के माध्यम से पुनरावृति करें
foreach (AttachedFile file in nodes)
{
    // संलग्न फ़ाइल को स्ट्रीम ऑब्जेक्ट में लोड करें
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // एक स्थानीय फ़ाइल बनाएँ
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // फ़ाइल स्ट्रीम कॉपी करें
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### यह सभी देखें

* class [AttachedFile](../)
* नाम स्थान [Aspose.Note](../../attachedfile/)
* सभा [Aspose.Note](../../../)


