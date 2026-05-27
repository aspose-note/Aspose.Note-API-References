---
title: "UnsupportedFileFormatException.FileFormat"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "UnsupportedFileFormatException property. يحصل على تنسيق الملف للبيانات الممررة إذا تم اكتشافه"
type: docs
weight: 10
url: /ar/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

يحصل على تنسيق الملف للبيانات الممررة إذا تم اكتشافه.

```csharp
public FileFormat FileFormat { get; }
```

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

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* namespace [Aspose.Note](../../unsupportedfileformatexception/)
* assembly [Aspose.Note](../../../)


