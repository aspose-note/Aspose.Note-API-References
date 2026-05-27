---
title: "PageSettings.Letter"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية PageSettings. يحصل على الإعدادات لصفحة تنسيق Letter"
type: docs
weight: 30
url: /ar/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

يحصل على الإعدادات لصفحة بتنسيق Letter.

```csharp
public static PageSettings Letter { get; }
```

## أمثلة

يوضح كيفية حفظ مستند بتنسيق Pdf مع تخطيط صفحة Letter.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// احفظ المستند.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

### انظر أيضًا

* class [PageSettings](../)
* namespace [Aspose.Note.Saving](../../pagesettings/)
* assembly [Aspose.Note](../../../)


