---
title: PdfSaveOptions.PageSplittingAlgorithm
second_title: Aspose.Note لمرجع NET API
description: PdfSaveOptions ملكية. الحصول على أو تعيين الخوارزمية المستخدمة لتقسيم الصفحات.
type: docs
weight: 50
url: /ar/net/aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/
---
## PdfSaveOptions.PageSplittingAlgorithm property

الحصول على أو تعيين الخوارزمية المستخدمة لتقسيم الصفحات.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### Property_Value

ملف`PageSplittingAlgorithm` .

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

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PdfSaveOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../pdfsaveoptions/)
* المجسم [Aspose.Note](../../../)


