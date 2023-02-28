---
title: Document.FileFormat
second_title: Aspose.Note لمرجع NET API
description: Document ملكية. الحصول على تنسيق الملف OneNote 2010  OneNote Online .
type: docs
weight: 60
url: /ar/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

الحصول على تنسيق الملف (OneNote 2010 ، OneNote Online) .

```csharp
public FileFormat FileFormat { get; }
```

### أمثلة

يوضح كيفية الحصول على تنسيق ملف لمستند.

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
        // معالجة OneNote عبر الإنترنت
        break;
}
```

### أنظر أيضا

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* مساحة الاسم [Aspose.Note](../../document/)
* المجسم [Aspose.Note](../../../)


