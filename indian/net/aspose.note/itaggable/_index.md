---
title: Interface ITaggable
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.ITaggable इंटरफेस. नड्स के लए इंटरफ़ेस जसे टैग द्वर चह्नत कय ज सकत है
type: docs
weight: 240
url: /hi/net/aspose.note/itaggable/
---
## ITaggable interface

नोड्स के लिए इंटरफ़ेस जिसे टैग द्वारा चिह्नित किया जा सकता है।

```csharp
public interface ITaggable : INode
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Tags](../../aspose.note/itaggable/tags/) { get; } | सभी टैग्स की सूची प्राप्त करता है। |

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

दिखाता है कि 'प्रोजेक्ट सी' से संबंधित सभी चेकबॉक्स आइटम को कैसे पूरा किया जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ को Aspose.Note में लोड करें।
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

दिखाता है कि 'प्रोजेक्ट सी' से संबंधित सभी चेकबॉक्स आइटम कैसे खोलें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ को Aspose.Note में लोड करें।
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

दिखाता है कि पिछले सप्ताह के दौरान अधूरे चेकबॉक्स द्वारा चिह्नित और बनाए गए आइटम वाले पृष्ठों वाले पीडीएफ को कैसे उत्पन्न किया जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ को Aspose.Note में लोड करें।
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<CheckBox>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteLastWeekReport.pdf"));
```

दिखाता है कि इस सप्ताह पूरा करने के लिए आउटलुक अपूर्ण कार्यों वाले पृष्ठों वाले पीडीएफ को कैसे उत्पन्न किया जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ को Aspose.Note में लोड करें।
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
var endOfWeek = DateTime.Today.AddDays(5 - (int)DateTime.Today.DayOfWeek);
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<NoteTask>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime && x.DueDate <= endOfWeek)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteTasksForThisWeekReport.pdf"));
```

### यह सभी देखें

* interface [INode](../inode/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


