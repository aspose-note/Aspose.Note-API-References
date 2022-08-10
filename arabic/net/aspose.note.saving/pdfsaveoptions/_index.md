---
title: PdfSaveOptions
second_title: Aspose.Note لمرجع NET API
description: يسمح بتحديد خيارات إضافية عند تقديم صفحات المستند إلى PDF .
type: docs
weight: 820
url: /ar/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

يسمح بتحديد خيارات إضافية عند تقديم صفحات المستند إلى PDF .

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | الحصول على أو تعيين إعدادات الخط لاستخدامها أثناء الحفظ |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression) { get; set; } | الحصول على أو تحديد نوع الضغط المطبق على الصور في ملف PDF. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality) { get; set; } | الحصول على أو تعيين قيمة تحدد جودة صور JPEG داخل مستند PDF . قد تختلف القيمة من 0 إلى 100 حيث يعني 0 أسوأ جودة ولكن أقصى ضغط ويعني 100 أفضل جودة ولكن أقل ضغط . |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | الحصول على أو تحديد عدد الصفحات المراد حفظها. افتراضيا هوMaxValue مما يعني أنه سيتم تقديم جميع صفحات المستند. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | الحصول على أو تحديد فهرس الصفحة الأولى للحفظ. بشكل افتراضي هو 0. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm) { get; set; } | الحصول على أو تعيين الخوارزمية المستخدمة لتقسيم الصفحات. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | يحصل على التنسيق الذي تم حفظ المستند به. |

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

عندما يتم حفظ صفحات OneNote الطويلة بتنسيق pdf ، يتم تقسيمها عبر الصفحات. يوضح النموذج كيفية تكوين منطق تقسيم الكائنات الموجودة في فواصل الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

يوضح كيفية حفظ مستند بتنسيق pdf.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // تعيين فهرس الصفحة للصفحة الأولى ليتم حفظها
                              PageIndex = 0,

                              // تعيين عدد الصفحات
                              PageCount = 1,
                          };

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام إعدادات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // استخدم ضغط Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // جودة ضغط JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions)
* مساحة الاسم [Aspose.Note.Saving](../../aspose.note.saving)
* المجسم [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
