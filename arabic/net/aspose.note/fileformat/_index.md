---
title: "تعداد FileFormat"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "Aspose.Note.FileFormat enum. يمثل تنسيق ملف OneNote"
type: docs
weight: 90
url: /ar/net/aspose.note/fileformat/
---
## FileFormat enumeration

يمثل تنسيق ملف OneNote.

```csharp
public enum FileFormat
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Unknown | `0` | تنسيق ملف غير معروف. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote Online. |

## أمثلة

يعرض كيفية التحقق مما إذا فشل تحميل المستند لأن تنسيق OneNote 2007 غير مدعوم.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

### انظر أيضًا

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


