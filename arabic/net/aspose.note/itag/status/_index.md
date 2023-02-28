---
title: ITag.Status
second_title: Aspose.Note لمرجع NET API
description: ITag ملكية. الحصول على الحالة أو تعيينها .
type: docs
weight: 50
url: /ar/net/aspose.note/itag/status/
---
## ITag.Status property

الحصول على الحالة أو تعيينها .

```csharp
public TagStatus Status { get; }
```

### Property_Value

ملف[`TagStatus`](../../tagstatus/) .

### أمثلة

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

يوضح كيفية الوصول إلى تفاصيل العلامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "TagFile.one");

// احصل على جميع عقد RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// كرر خلال كل عقدة
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // استرداد الخصائص
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

### أنظر أيضا

* enum [TagStatus](../../tagstatus/)
* interface [ITag](../)
* مساحة الاسم [Aspose.Note](../../itag/)
* المجسم [Aspose.Note](../../../)


