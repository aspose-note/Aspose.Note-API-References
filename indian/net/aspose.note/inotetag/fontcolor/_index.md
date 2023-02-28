---
title: INoteTag.FontColor
second_title: Aspose.Note .NET API संदर्भ के लिए
description: INoteTag संपत्त. फ़न्ट रंग प्रप्त य सेट करत है
type: docs
weight: 10
url: /hi/net/aspose.note/inotetag/fontcolor/
---
## INoteTag.FontColor property

फ़ॉन्ट रंग प्राप्त या सेट करता है।

```csharp
public Color FontColor { get; set; }
```

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

* interface [INoteTag](../)
* नाम स्थान [Aspose.Note](../../inotetag/)
* सभा [Aspose.Note](../../../)


