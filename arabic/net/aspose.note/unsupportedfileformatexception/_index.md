---
title: "فئة UnsupportedFileFormatException"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "Aspose.Note.UnsupportedFileFormatException فئة. تُرمى أثناء تحميل المستند عندما لا يتم التعرف على تنسيق الملف أو لا يدعمه Aspose.Note"
type: docs
weight: 1070
url: /ar/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

يُرمى أثناء تحميل المستند، عندما لا يتم التعرف على تنسيق الملف أو لا يدعمه Aspose.Note.

```csharp
public class UnsupportedFileFormatException : Exception
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | يحصل على تنسيق الملف للبيانات الممررة إذا تم اكتشافه. |

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


