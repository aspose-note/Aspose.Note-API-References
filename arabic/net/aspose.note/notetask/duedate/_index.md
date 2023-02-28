---
title: NoteTask.DueDate
second_title: Aspose.Note لمرجع NET API
description: NoteTask ملكية. الحصول على تاريخ الاستحقاق أو تحديده.
type: docs
weight: 70
url: /ar/net/aspose.note/notetask/duedate/
---
## NoteTask.DueDate property

الحصول على تاريخ الاستحقاق أو تحديده.

```csharp
public DateTime DueDate { get; set; }
```

### Property_Value

ملفDateTime .

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

يوضح كيفية الوصول إلى تفاصيل مهام Outlook.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tasks();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على جميع عقد RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// كرر خلال كل عقدة
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // استرداد الخصائص
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### أنظر أيضا

* class [NoteTask](../)
* مساحة الاسم [Aspose.Note](../../notetask/)
* المجسم [Aspose.Note](../../../)


