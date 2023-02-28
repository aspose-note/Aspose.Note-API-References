---
title: Class NoteTask
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.NoteTask कक्ष. एक नट कर्य क प्रतनधत्व करत है
type: docs
weight: 400
url: /hi/net/aspose.note/notetask/
---
## NoteTask class

एक नोट कार्य का प्रतिनिधित्व करता है।

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | एक मान प्राप्त करता है जो इंगित करता है कि चेकबॉक्स चेक किए गए राज्य में है या नहीं। |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | पूर्ण समय प्राप्त या सेट करता है। |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | निर्माण समय प्राप्त या सेट करता है। |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | देय तिथि प्राप्त या सेट करता है। |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | आइकन प्राप्त करता है या सेट करता है। |
| [Label](../../aspose.note/checkbox/label/) { get; } | लेबल पाठ प्राप्त करता है। |
| [Status](../../aspose.note/checkbox/status/) { get; } | स्थिति प्राप्त या सेट करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | NoFollowUpDateFlag आइकन और निर्दिष्ट देय तिथि के साथ एक नया नोट कार्य बनाता है। |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | FollowUpNextWeekFlag आइकन के साथ एक नया नोट कार्य बनाता है। |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | FollowUpThisWeekFlag आइकन के साथ एक नया नोट कार्य बनाता है। |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | FollowUpTodayFlag आइकन के साथ एक नया नोट कार्य बनाता है। |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | FollowUpTomorrowFlag आइकन के साथ एक नया नोट कार्य बनाता है। |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | NoFollowUpDateFlag आइकन के साथ एक नया नोट कार्य बनाता है। |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | निर्धारित करता है कि निर्दिष्ट वस्तु वर्तमान वस्तु के बराबर है या नहीं। |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | निर्धारित करता है कि निर्दिष्ट वस्तु वर्तमान वस्तु के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | प्रकार के लिए हैश फ़ंक्शन के रूप में कार्य करता है। |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | वर्तमान समय को पूर्ण समय के रूप में उपयोग करके पूर्ण स्थिति में टैग सेट करता है। |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | टैग को पूर्ण स्थिति पर सेट करता है। |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | टैग को ओपन स्टेट पर सेट करता है। |

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

* class [CheckBox](../checkbox/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


