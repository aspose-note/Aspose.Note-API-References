---
title: "Image.LastModifiedTime"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Image. تحصل أو تعين وقت التعديل الأخير"
type: docs
weight: 130
url: /ar/net/aspose.note/image/lastmodifiedtime/
---
## Image.LastModifiedTime property

يحصل أو يعيّن وقت التعديل الأخير.

```csharp
public DateTime LastModifiedTime { get; set; }
```

## أمثلة

يظهر كيفية الحصول على معلومات ميتا للصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// الحصول على جميع عقد Image
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


