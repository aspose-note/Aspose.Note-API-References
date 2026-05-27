---
title: "الفئة PdfSaveOptions"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Saving.PdfSaveOptions. تسمح بتحديد خيارات إضافية عند تحويل صفحات المستند إلى PDF"
type: docs
weight: 930
url: /ar/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

يسمح بتحديد خيارات إضافية عند تحويل صفحات المستند إلى PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | يحصل أو يضبط إعدادات الخط التي سيتم استخدامها أثناء الحفظ |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression/) { get; set; } | يحصل أو يضبط نوع الضغط المطبق على الصور في ملف PDF. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality/) { get; set; } | يحصل أو يضبط قيمة تحدد جودة صور JPEG داخل مستند PDF. يمكن أن تتراوح القيمة من 0 إلى 100 حيث 0 تعني أسوأ جودة ولكن أقصى ضغط و100 تعني أفضل جودة ولكن أقل ضغط. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | يحصل أو يضبط عدد الصفحات التي سيتم حفظها. القيمة الافتراضية هي MaxValue مما يعني أنه سيتم عرض جميع صفحات المستند. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | يحصل أو يضبط فهرس الصفحة الأولى التي سيتم حفظها. القيمة الافتراضية هي 0. |
| [PageSettings](../../aspose.note.saving/pdfsaveoptions/pagesettings/) { get; set; } | يحصل أو يضبط إعدادات الصفحة لكل صفحة في المستند. بشكل افتراضي يعتمد على CurrentUICulture، *الثقافات الأمريكية تستخدم إعداد الحرف، والبقية تستخدم إعداد A4. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/) { get; set; } | يحصل أو يضبط الخوارزمية المستخدمة لتقسيم الصفحات. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | يحصل على الصيغة التي يُحفظ بها المستند. |

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

يوضح كيفية حفظ الدفتر بتنسيق pdf مع الخيارات المحددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// احفظ الدفتر
notebook.Save(dataDir, notebookSaveOptions);
```

عند حفظ صفحات OneNote الطويلة بتنسيق pdf يتم تقسيمها عبر صفحات. يوضح المثال كيفية تكوين منطق التقسيم للكائنات الموجودة على فواصل الصفحات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

يظهر كيفية حفظ مستند بتنسيق pdf.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // تعيين فهرس الصفحة الأولى التي سيتم حفظها
                              PageIndex = 0,

                              // تعيين عدد الصفحات
                              PageCount = 1,
                          };

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

يظهر كيفية حفظ مستند بتنسيق pdf باستخدام إعدادات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // استخدام ضغط Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // جودة ضغط JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

عند حفظ صفحات OneNote الطويلة بتنسيق PDF يتم تقسيمها عبر صفحات متعددة. يوضح المثال كيفية تكوين منطق التقسيم للكائنات الموجودة على فواصل الصفحات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
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

### انظر أيضًا

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


