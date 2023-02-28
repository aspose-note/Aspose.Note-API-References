---
title: Class KeepSolidObjectsAlgorithm
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Saving.KeepSolidObjectsAlgorithm فصل. ينقل الكائن بالكامل إلى الصفحة التالية في حالة عدم احتوائه في الصفحة الأصلية.
type: docs
weight: 740
url: /ar/net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

ينقل الكائن بالكامل إلى الصفحة التالية في حالة عدم احتوائه في الصفحة الأصلية.

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | يقوم بتهيئة مثيل جديد لملف`KeepSolidObjectsAlgorithm` فئة تستخدم حد الارتفاع الافتراضي للجزء المستنسخ. |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | يقوم بتهيئة مثيل جديد لملف`KeepSolidObjectsAlgorithm` فئة باستخدام حد ارتفاع معين للجزء المستنسخ. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | يحصل على حد ارتفاع الجزء المستنسخ. |

## مجالات

| اسم | وصف |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | الحجم الأقصى الافتراضي للجزء المستنسخ. |

### أمثلة

يوضح كيفية حفظ دفتر الملاحظات بتنسيق pdf بخيارات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// حفظ دفتر الملاحظات
notebook.Save(dataDir, notebookSaveOptions);
```

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

عندما يتم حفظ صفحات OneNote الطويلة بتنسيق pdf ، يتم تقسيمها عبر الصفحات. يوضح المثال كيفية تكوين منطق تقسيم الكائنات الموجودة في فواصل الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### أنظر أيضا

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* مساحة الاسم [Aspose.Note.Saving](../../aspose.note.saving/)
* المجسم [Aspose.Note](../../)


