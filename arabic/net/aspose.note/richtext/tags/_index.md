---
title: "RichText.Tags"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية RichText. يحصل على قائمة بجميع العلامات في فقرة"
type: docs
weight: 120
url: /ar/net/aspose.note/richtext/tags/
---
## RichText.Tags property

يحصل على قائمة جميع العلامات في الفقرة.

```csharp
public List<ITag> Tags { get; }
```

## أمثلة

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

* interface [ITag](../../itag/)
* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)


