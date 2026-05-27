---
title: "AttachedFile.Bytes"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية AttachedFile. يحصل على البيانات الثنائية لملف مضمّن"
type: docs
weight: 50
url: /ar/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

يحصل على البيانات الثنائية لملف مضمّن.

```csharp
public byte[] Bytes { get; }
```

## أمثلة

يظهر كيفية الحصول على محتوى ملف مرفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Attachments();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الملفات المرفقة
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// تكرار عبر جميع العقد
foreach (AttachedFile file in nodes)
{
    // تحميل الملف المرفق إلى كائن تدفق
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // إنشاء ملف محلي
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // نسخ تدفق الملف
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### انظر أيضًا

* class [AttachedFile](../)
* namespace [Aspose.Note](../../attachedfile/)
* assembly [Aspose.Note](../../../)


