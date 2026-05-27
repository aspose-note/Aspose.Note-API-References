---
title: "الفئة PageSettings"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Saving.PageSettings. تمثل إعدادات التخطيط لصفحة"
type: docs
weight: 900
url: /ar/net/aspose.note.saving/pagesettings/
---
## PageSettings class

يمثل إعدادات التخطيط لصفحة.

```csharp
public class PageSettings
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | يحصل على الإعدادات لصفحة بتنسيق A4. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | يحصل على الإعدادات لصفحة بتنسيق A4 ذات ارتفاع غير محدود. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | يحصل على الإعدادات لصفحة بتنسيق Letter. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | يحصل على الإعدادات لصفحة بتنسيق Letter ذات ارتفاع غير محدود. |

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

يوضح كيفية حفظ مستند بتنسيق Pdf مع تخطيط صفحة A4 دون حد للارتفاع.

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

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


