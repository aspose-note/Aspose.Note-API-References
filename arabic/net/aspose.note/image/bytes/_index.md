---
title: "Image.Bytes"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Image. تحصل على مخزن بيانات الصورة"
type: docs
weight: 50
url: /ar/net/aspose.note/image/bytes/
---
## Image.Bytes property

يحصل على مخزن بيانات الصورة.

```csharp
public byte[] Bytes { get; }
```

## أمثلة

يظهر كيفية الحصول على صورة من مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// الحصول على جميع عقد Image
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // حفظ بايتات الصورة إلى ملف
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### انظر أيضًا

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


