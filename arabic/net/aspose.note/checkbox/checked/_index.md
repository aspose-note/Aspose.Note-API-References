---
title: CheckBox.Checked
second_title: Aspose.Note لمرجع NET API
description: CheckBox ملكية. يحصل على قيمة تشير إلى ما إذا كان CheckBox في الحالة المحددة.
type: docs
weight: 10
url: /ar/net/aspose.note/checkbox/checked/
---
## CheckBox.Checked property

يحصل على قيمة تشير إلى ما إذا كان CheckBox في الحالة المحددة.

```csharp
public bool Checked { get; }
```

### أمثلة

يوضح كيفية إنشاء ملف pdf يحتوي على جميع الصفحات المتعلقة بالمشروع أ.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// قم بتحميل المستند في Aspose.
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

يوضح كيفية إكمال جميع عناصر مربعات الاختيار المتعلقة بالمشروع ج.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// قم بتحميل المستند في Aspose.
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

يوضح كيفية فتح جميع عناصر مربعات الاختيار المتعلقة بالمشروع ج.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// قم بتحميل المستند في Aspose.
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

يوضح كيفية إنشاء ملف pdf يحتوي على صفحات تحتوي على عناصر تم تمييزها بخانات اختيار غير مكتملة وتم إنشاؤها خلال الأسبوع الماضي.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// قم بتحميل المستند في Aspose.
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

يوضح كيفية إنشاء ملف pdf يحتوي على صفحات بها مهام غير مكتملة في Outlook لإكمالها في هذا الأسبوع.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// قم بتحميل المستند في Aspose.
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

### أنظر أيضا

* class [CheckBox](../)
* مساحة الاسم [Aspose.Note](../../checkbox/)
* المجسم [Aspose.Note](../../../)


