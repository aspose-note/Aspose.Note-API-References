---
title: "Image.OriginalWidth"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية Image. تحصل على العرض الأصلي. هذا هو العرض الأصلي للصورة قبل تغيير الحجم"
type: docs
weight: 150
url: /ar/net/aspose.note/image/originalwidth/
---
## Image.OriginalWidth property

يحصل على العرض الأصلي. هذا هو العرض الأصلي للصورة، قبل تغيير الحجم.

```csharp
public float OriginalWidth { get; }
```

## أمثلة

يوضح كيفية الحصول على معلومات ميتا للصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على جميع عقد Image
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

### انظر أيضًا

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


