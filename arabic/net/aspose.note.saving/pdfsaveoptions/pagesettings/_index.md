---
title: "PdfSaveOptions.PageSettings"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "خاصية PdfSaveOptions. يحصل أو يضبط إعدادات الصفحة لكل صفحة في المستند. بشكل افتراضي يعتمد على CurrentUICulture؛ الثقافات الأمريكية تستخدم إعداد Letter بينما الأخرى تستخدم إعداد A4."
type: docs
weight: 40
url: /ar/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

يحصل أو يعيّن إعدادات الصفحة لكل صفحة في المستند. بشكل افتراضي يعتمد على CurrentUICulture، *الثقافات الأمريكية لديها إعداد الحرف، والثقافات الأخرى لديها إعداد A4.

```csharp
public PageSettings PageSettings { get; set; }
```

## أمثلة

يعرض كيفية حفظ مستند بتنسيق Pdf مع تخطيط صفحة Letter.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// احفظ المستند.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

يعرض كيفية حفظ مستند بتنسيق Pdf مع تخطيط صفحة A4 دون حد للارتفاع.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// احفظ المستند.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### انظر أيضًا

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Note.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Note](../../../)


