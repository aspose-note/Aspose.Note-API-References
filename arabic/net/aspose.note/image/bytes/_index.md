---
title: Image.Bytes
second_title: Aspose.Note لمرجع NET API
description: Image ملكية. يحصل على مخزن بيانات الصورة.
type: docs
weight: 50
url: /ar/net/aspose.note/image/bytes/
---
## Image.Bytes property

يحصل على مخزن بيانات الصورة.

```csharp
public byte[] Bytes { get; }
```

### أمثلة

يوضح كيفية الحصول على صورة من مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على جميع عُقد الصور
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // حفظ بايت الصورة في ملف
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### أنظر أيضا

* class [Image](../)
* مساحة الاسم [Aspose.Note](../../image/)
* المجسم [Aspose.Note](../../../)


