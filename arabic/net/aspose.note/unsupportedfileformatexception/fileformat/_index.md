---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note لمرجع NET API
description: UnsupportedFileFormatException ملكية. يحصل على تنسيق ملف البيانات التي تم تمريرها في حالة اكتشافه.
type: docs
weight: 10
url: /ar/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

يحصل على تنسيق ملف البيانات التي تم تمريرها في حالة اكتشافه.

```csharp
public FileFormat FileFormat { get; }
```

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

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* مساحة الاسم [Aspose.Note](../../unsupportedfileformatexception/)
* المجسم [Aspose.Note](../../../)


