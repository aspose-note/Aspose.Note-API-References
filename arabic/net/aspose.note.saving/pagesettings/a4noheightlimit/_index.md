---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note لمرجع NET API
description: PageSettings ملكية. الحصول على إعدادات لصفحة تنسيق A4 بارتفاع غير محدود .
type: docs
weight: 20
url: /ar/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

الحصول على إعدادات لصفحة تنسيق A4 بارتفاع غير محدود .

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### أمثلة

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

* class [PageSettings](../)
* مساحة الاسم [Aspose.Note.Saving](../../pagesettings/)
* المجسم [Aspose.Note](../../../)


