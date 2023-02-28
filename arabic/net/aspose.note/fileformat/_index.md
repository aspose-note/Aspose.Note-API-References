---
title: Enum FileFormat
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.FileFormat تعداد. يمثل تنسيق ملف OneNote .
type: docs
weight: 90
url: /ar/net/aspose.note/fileformat/
---
## FileFormat enumeration

يمثل تنسيق ملف OneNote .

```csharp
public enum FileFormat
```

### قيم

| اسم | قيمة | وصف |
| --- | --- | --- |
| Unknown | `0` | تنسيق ملف غير معروف . |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote Online. |

### أمثلة

يوضح كيفية التحقق من فشل تحميل المستند لأن تنسيق OneNote 2007 غير مدعوم.

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

### أنظر أيضا

* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


