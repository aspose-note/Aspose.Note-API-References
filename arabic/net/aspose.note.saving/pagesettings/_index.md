---
title: Class PageSettings
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Saving.PageSettings فصل. يمثل إعدادات التخطيط للصفحة.
type: docs
weight: 820
url: /ar/net/aspose.note.saving/pagesettings/
---
## PageSettings class

يمثل إعدادات التخطيط للصفحة.

```csharp
public class PageSettings
```

## الخصائص

| اسم | وصف |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | الحصول على إعدادات لصفحة تنسيق A4 . |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | الحصول على إعدادات لصفحة تنسيق A4 بارتفاع غير محدود . |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | الحصول على إعدادات لصفحة تنسيق Letter . |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | الحصول على إعدادات لصفحة تنسيق Letter بارتفاع غير محدود. |

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

* مساحة الاسم [Aspose.Note.Saving](../../aspose.note.saving/)
* المجسم [Aspose.Note](../../)


