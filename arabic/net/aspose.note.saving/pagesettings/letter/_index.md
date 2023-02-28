---
title: PageSettings.Letter
second_title: Aspose.Note لمرجع NET API
description: PageSettings ملكية. الحصول على إعدادات لصفحة تنسيق Letter .
type: docs
weight: 30
url: /ar/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

الحصول على إعدادات لصفحة تنسيق Letter .

```csharp
public static PageSettings Letter { get; }
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

### أنظر أيضا

* class [PageSettings](../)
* مساحة الاسم [Aspose.Note.Saving](../../pagesettings/)
* المجسم [Aspose.Note](../../../)


