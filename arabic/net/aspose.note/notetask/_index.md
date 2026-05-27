---
title: "الفئة NoteTask"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "Aspose.Note.NoteTask الفئة. يمثل مهمة ملاحظة"
type: docs
weight: 470
url: /ar/net/aspose.note/notetask/
---
## NoteTask class

يمثل مهمة ملاحظة.

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | يحصل على قيمة تشير إلى ما إذا كان CheckBox في الحالة المحددة. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | يحصل أو يعيّن وقت الإكمال. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | يحصل أو يعيّن وقت الإنشاء. |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | يحصل أو يضبط تاريخ الاستحقاق. |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | يحصل أو يعيّن الأيقونة. |
| [Label](../../aspose.note/checkbox/label/) { get; } | يحصل على نص التسمية. |
| [Status](../../aspose.note/checkbox/status/) { get; } | يحصل أو يعيّن الحالة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | ينشئ مهمة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag وتاريخ استحقاق محدد. |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | ينشئ مهمة ملاحظة جديدة مع أيقونة FollowUpNextWeekFlag. |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | ينشئ مهمة ملاحظة جديدة مع أيقونة FollowUpThisWeekFlag. |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | ينشئ مهمة ملاحظة جديدة مع أيقونة FollowUpTodayFlag. |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | ينشئ مهمة ملاحظة جديدة مع أيقونة FollowUpTomorrowFlag. |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | ينشئ مهمة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag. |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | يعمل كدالة تجزئة للنوع. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | يضبط العلامة إلى حالة مكتملة باستخدام الوقت الحالي كوقت إكمال. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | يضبط العلامة إلى حالة مكتملة. |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | يضبط العلامة إلى حالة مفتوحة. |

## أمثلة

يوضح كيفية إنشاء ملف pdf يحتوي على جميع الصفحات المتعلقة بـ 'Project A'.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// حمّل المستند إلى Aspose.Note.
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

يوضح كيفية الوصول إلى تفاصيل مهام outlook.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tasks();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على جميع عقد RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// تكرار عبر كل عقدة
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // استرجاع الخصائص
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### انظر أيضًا

* class [CheckBox](../checkbox/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


