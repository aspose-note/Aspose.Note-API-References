---
title: NoteTask.DueDate
second_title: Aspose.Note .NET API संदर्भ के लिए
description: NoteTask संपत्त. देय तथ प्रप्त य सेट करत है
type: docs
weight: 70
url: /hi/net/aspose.note/notetask/duedate/
---
## NoteTask.DueDate property

देय तिथि प्राप्त या सेट करता है।

```csharp
public DateTime DueDate { get; set; }
```

### संपत्ति मूल्य

दDateTime .

### उदाहरण

दिखाता है कि 'प्रोजेक्ट ए' से संबंधित सभी पृष्ठों वाली पीडीएफ कैसे उत्पन्न करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ को Aspose.Note में लोड करें।
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.Any(x => x.Label.Contains("Project A"))))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "ProjectA_Report.pdf"));
```

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

* class [NoteTask](../)
* नाम स्थान [Aspose.Note](../../notetask/)
* सभा [Aspose.Note](../../../)


