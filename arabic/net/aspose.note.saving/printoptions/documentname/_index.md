---
title: PrintOptions.DocumentName
second_title: Aspose.Note لمرجع NET API
description: PrintOptions ملكية. الحصول على أو تحديد اسم المستند المطلوب عرضه على سبيل المثال  في مربع حوار حالة الطباعة أو قائمة انتظار الطابعة أثناء طباعة المستند.
type: docs
weight: 20
url: /ar/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

الحصول على أو تحديد اسم المستند المطلوب عرضه (على سبيل المثال ، في مربع حوار حالة الطباعة أو قائمة انتظار الطابعة) أثناء طباعة المستند.

```csharp
public string DocumentName { get; set; }
```

### أمثلة

يوضح كيفية إرسال المستند إلى الطابعة باستخدام مربع حوار Windows القياسي مع خيارات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

### أنظر أيضا

* class [PrintOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../printoptions/)
* المجسم [Aspose.Note](../../../)


