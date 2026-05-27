---
title: "الفئة PrintOptions"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Saving.PrintOptions. خيارات تُستخدم لطباعة مستند."
type: docs
weight: 940
url: /ar/net/aspose.note.saving/printoptions/
---
## PrintOptions class

الخيارات المستخدمة لطباعة مستند.

```csharp
public class PrintOptions
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [PrintOptions](printoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | يحصل أو يعيّن اسم المستند للعرض (على سبيل المثال، في مربع حوار حالة الطباعة أو في طابور الطابعة) أثناء طباعة المستند. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | يحصل أو يضبط الخوارزمية المستخدمة لتقسيم الصفحات. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | يحصل أو يعيّن إعدادات الطابعة. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | يحصل أو يضبط الدقة للصور المُولَّدة، بوحدة النقاط في البوصة. |

## أمثلة

يظهر كيفية إرسال المستند إلى طابعة باستخدام مربع حوار Windows القياسي مع الخيارات المحددة.

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

### انظر أيضًا

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


