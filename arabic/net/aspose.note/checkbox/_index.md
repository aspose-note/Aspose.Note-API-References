---
title: "الفئة CheckBox"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "الفئة Aspose.Note.CheckBox. الفئة الأساسية للعلامات التي يمكنها تبديل حالتها بين مكتمل وغير مكتمل"
type: docs
weight: 20
url: /ar/net/aspose.note/checkbox/
---
## CheckBox class

الفئة الأساسية للوسوم التي يمكنها تبديل حالتها بين مكتملة وغير مكتملة.

```csharp
public abstract class CheckBox : ITag
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | يحصل على قيمة تشير إلى ما إذا كان CheckBox في الحالة المحددة. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | الحصول على أو تعيين وقت الانتهاء. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | الحصول على أو تعيين وقت الإنشاء. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | الحصول على أو تعيين الأيقونة. |
| [Label](../../aspose.note/checkbox/label/) { get; } | يحصل على نص التسمية. |
| [Status](../../aspose.note/checkbox/status/) { get; } | الحصول على أو تعيين الحالة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | تعيين العلامة إلى حالة مكتملة باستخدام الوقت الحالي كوقت إكمال. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | تعيين العلامة إلى حالة مكتملة. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | تعيين العلامة إلى حالة مفتوحة. |

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

يوضح كيفية إكمال جميع عناصر خانة الاختيار المرتبطة بـ 'Project C'.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// حمّل المستند إلى Aspose.Note.
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

يوضح كيفية فتح جميع عناصر خانة الاختيار المرتبطة بـ 'Project C'.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// حمّل المستند إلى Aspose.Note.
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

يوضح كيفية إنشاء ملف PDF يحتوي على صفحات بها عناصر محددة بخانات اختيار غير مكتملة وتم إنشاؤها خلال الأسبوع الماضي.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// حمّل المستند إلى Aspose.Note.
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

يوضح كيفية إنشاء ملف PDF يحتوي على صفحات بها مهام Outlook غير مكتملة لإكمالها هذا الأسبوع.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// حمّل المستند إلى Aspose.Note.
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

### انظر أيضًا

* interface [ITag](../itag/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


