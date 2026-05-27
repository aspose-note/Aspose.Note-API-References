---
title: "PageSettings.A4NoHeightLimit"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية PageSettings. يحصل على الإعدادات لصفحة تنسيق A4 بدون حد للارتفاع"
type: docs
weight: 20
url: /ar/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

يحصل على الإعدادات لصفحة بتنسيق A4 ذات ارتفاع غير محدود.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

## أمثلة

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

* class [PageSettings](../)
* namespace [Aspose.Note.Saving](../../pagesettings/)
* assembly [Aspose.Note](../../../)


