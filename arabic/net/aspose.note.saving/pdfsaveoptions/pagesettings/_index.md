---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note لمرجع NET API
description: PdfSaveOptions ملكية. الحصول على إعدادات الصفحة أو تعيينها لكل صفحة في المستند. بشكل افتراضي يعتمد على CurrentUICulture   ثقافات الولايات المتحدة بها إعداد الحروف  والبعض الآخر بها إعدادات A4.
type: docs
weight: 40
url: /ar/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

الحصول على إعدادات الصفحة أو تعيينها لكل صفحة في المستند. بشكل افتراضي يعتمد على CurrentUICulture ، * ثقافات الولايات المتحدة بها إعداد الحروف ، والبعض الآخر بها إعدادات A4.

```csharp
public PageSettings PageSettings { get; set; }
```

### أمثلة

يوضح كيفية حفظ مستند بتنسيق Pdf مع تخطيط صفحة الرسالة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// احفظ المستند.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

يوضح كيفية حفظ مستند بتنسيق Pdf مع تخطيط صفحة A4 بدون حد للارتفاع.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// احفظ المستند.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### أنظر أيضا

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../pdfsaveoptions/)
* المجسم [Aspose.Note](../../../)


