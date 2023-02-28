---
title: RichText.Tags
second_title: Aspose.Note .NET API संदर्भ के लिए
description: RichText संपत्त. अनुच्छेद के सभ टैग क सूच प्रप्त करत है
type: docs
weight: 90
url: /hi/net/aspose.note/richtext/tags/
---
## RichText.Tags property

अनुच्छेद के सभी टैग की सूची प्राप्त करता है।

```csharp
public List<ITag> Tags { get; }
```

### उदाहरण

दिखाता है कि आउटलुक के कार्यों के विवरण तक कैसे पहुंचा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tasks();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// सभी रिचटेक्स्ट नोड्स प्राप्त करें
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// प्रत्येक नोड के माध्यम से दोहराएं
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // गुणों को पुनः प्राप्त करें
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### यह सभी देखें

* interface [ITag](../../itag/)
* class [RichText](../)
* नाम स्थान [Aspose.Note](../../richtext/)
* सभा [Aspose.Note](../../../)


