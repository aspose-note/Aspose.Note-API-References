---
title: Interface INoteTag
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.INoteTag واجهه المستخدم. واجهة علامات الملاحظات أي العلامات غير المرتبطة بمهام Outlook .
type: docs
weight: 180
url: /ar/net/aspose.note/inotetag/
---
## INoteTag interface

واجهة علامات الملاحظات (أي العلامات غير المرتبطة بمهام Outlook) .

```csharp
public interface INoteTag : ITag
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | الحصول على لون الخط أو تعيينه. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | الحصول على لون التمييز أو تعيينه. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | الحصول على نص التسمية أو تعيينه. |

### أمثلة

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

* interface [ITag](../itag/)
* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


