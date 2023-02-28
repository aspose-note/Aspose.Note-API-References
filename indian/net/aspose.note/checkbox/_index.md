---
title: Class CheckBox
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.CheckBox कक्ष. टैग के लए आधर वर्ग ज अपन स्थत क पूर्ण और अपूर्ण के बच टगल कर सकत है
type: docs
weight: 20
url: /hi/net/aspose.note/checkbox/
---
## CheckBox class

टैग के लिए आधार वर्ग जो अपनी स्थिति को पूर्ण और अपूर्ण के बीच टॉगल कर सकता है।

```csharp
public abstract class CheckBox : ITag
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | एक मान प्राप्त करता है जो इंगित करता है कि चेकबॉक्स चेक किए गए राज्य में है या नहीं। |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | पूर्ण समय प्राप्त या सेट करता है। |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | निर्माण समय प्राप्त या सेट करता है। |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | आइकन प्राप्त करता है या सेट करता है। |
| [Label](../../aspose.note/checkbox/label/) { get; } | लेबल पाठ प्राप्त करता है। |
| [Status](../../aspose.note/checkbox/status/) { get; } | स्थिति प्राप्त या सेट करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | वर्तमान समय को पूर्ण समय के रूप में उपयोग करके पूर्ण स्थिति में टैग सेट करता है। |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | टैग को पूर्ण स्थिति पर सेट करता है। |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | टैग को ओपन स्टेट पर सेट करता है। |

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

* interface [ITag](../itag/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


