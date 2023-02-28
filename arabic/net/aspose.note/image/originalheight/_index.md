---
title: Image.OriginalHeight
second_title: Aspose.Note لمرجع NET API
description: Image ملكية. الحصول على الارتفاع الأصلي. هذا هو العرض الأصلي للصورة قبل تغيير الحجم.
type: docs
weight: 140
url: /ar/net/aspose.note/image/originalheight/
---
## Image.OriginalHeight property

الحصول على الارتفاع الأصلي. هذا هو العرض الأصلي للصورة قبل تغيير الحجم.

```csharp
public float OriginalHeight { get; }
```

### أمثلة

يوضح كيفية الحصول على معلومات التعريف الخاصة بالصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على جميع عُقد الصور
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

### أنظر أيضا

* class [Image](../)
* مساحة الاسم [Aspose.Note](../../image/)
* المجسم [Aspose.Note](../../../)


