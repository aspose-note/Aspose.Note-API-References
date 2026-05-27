---
title: "INoteTag.FontColor"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية INoteTag. يحصل أو يضبط لون الخط"
type: docs
weight: 10
url: /ar/net/aspose.note/inotetag/fontcolor/
---
## INoteTag.FontColor property

يحصل أو يضبط لون الخط.

```csharp
public Color FontColor { get; set; }
```

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

* interface [INoteTag](../)
* namespace [Aspose.Note](../../inotetag/)
* assembly [Aspose.Note](../../../)


