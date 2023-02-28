---
title: Interface INoteTag
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.INoteTag इंटरफेस. नट टैग के लए इंटरफ़ेस यन टैग ज आउटलुक कर्यं से संबद्ध नहं हैं
type: docs
weight: 180
url: /hi/net/aspose.note/inotetag/
---
## INoteTag interface

नोट टैग के लिए इंटरफ़ेस (यानी टैग जो आउटलुक कार्यों से संबद्ध नहीं हैं)।

```csharp
public interface INoteTag : ITag
```

## गुण

| नाम | विवरण |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | फ़ॉन्ट रंग प्राप्त या सेट करता है। |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | हाइलाइट रंग प्राप्त या सेट करता है। |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | लेबल टेक्स्ट प्राप्त या सेट करता है. |

### उदाहरण

टैग के विवरण तक पहुंचने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "TagFile.one");

// सभी रिचटेक्स्ट नोड्स प्राप्त करें
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// प्रत्येक नोड के माध्यम से दोहराएं
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // गुणों को पुनः प्राप्त करें
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### यह सभी देखें

* interface [ITag](../itag/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


