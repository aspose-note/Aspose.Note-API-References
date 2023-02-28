---
title: Class UnsupportedFileFormatException
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.UnsupportedFileFormatException فصل. يتم إلقاؤه أثناء تحميل المستند  عندما لا يتم التعرف على تنسيق الملف أو عدم دعمه بواسطة Aspose.
type: docs
weight: 990
url: /ar/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

يتم إلقاؤه أثناء تحميل المستند ، عندما لا يتم التعرف على تنسيق الملف أو عدم دعمه بواسطة Aspose.

```csharp
public class UnsupportedFileFormatException : Exception
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | يحصل على تنسيق ملف البيانات التي تم تمريرها في حالة اكتشافه. |

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


