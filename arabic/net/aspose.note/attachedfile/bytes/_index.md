---
title: AttachedFile.Bytes
second_title: Aspose.Note لمرجع NET API
description: AttachedFile ملكية. يحصل على البيانات الثنائية لملف مضمن.
type: docs
weight: 50
url: /ar/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

يحصل على البيانات الثنائية لملف مضمن.

```csharp
public byte[] Bytes { get; }
```

### أمثلة

يوضح كيفية الحصول على محتوى ملف مرفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Attachments();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الملفات المرفقة
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// كرر عبر جميع العقد
foreach (AttachedFile file in nodes)
{
    // تحميل الملف المرفق إلى كائن تيار
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // إنشاء ملف محلي
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // نسخ الملف
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### أنظر أيضا

* class [AttachedFile](../)
* مساحة الاسم [Aspose.Note](../../attachedfile/)
* المجسم [Aspose.Note](../../../)


