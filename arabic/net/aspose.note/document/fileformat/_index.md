---
title: "Document.FileFormat"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Document. تحصل على تنسيق الملف OneNote 2010 OneNote Online"
type: docs
weight: 60
url: /ar/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

يحصل على تنسيق الملف (OneNote 2010، OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

## أمثلة

يعرض كيفية الحصول على تنسيق الملف للمستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // معالجة OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // معالجة OneNote Online
        break;
}
```

### انظر أيضًا

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


