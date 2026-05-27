---
title: "Interface INoteTag"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "واجهة Aspose.Note.INoteTag. الواجهة لعلامات الملاحظات أي العلامات التي لا ترتبط بمهام Outlook."
type: docs
weight: 180
url: /ar/net/aspose.note/inotetag/
---
## INoteTag interface

الواجهة لعلامات الملاحظات (أي العلامات التي لا ترتبط بمهام Outlook).

```csharp
public interface INoteTag : ITag
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | يحصل أو يضبط لون الخط. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | يحصل أو يضبط لون التظليل. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | يحصل أو يضبط نص التسمية. |

## أمثلة

يظهر كيفية الوصول إلى تفاصيل العلامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// احصل على جميع عقد RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// تكرار عبر كل عقدة
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // استرجاع الخصائص
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

### انظر أيضًا

* interface [ITag](../itag/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


