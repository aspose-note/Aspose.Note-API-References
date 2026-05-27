---
title: "الفئة NotebookPdfSaveOptions"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Saving.NotebookPdfSaveOptions. تسمح بتحديد خيارات إضافية عند تحويل صفحات الدفتر إلى PDF"
type: docs
weight: 860
url: /ar/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

يسمح بتحديد خيارات إضافية عند تحويل صفحات الدفتر إلى PDF.

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب حفظ المستندات الفرعية صراحةً. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان هيكل الأطفال في الدفتر يُحفظ مسطحًا. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

## أمثلة

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

### انظر أيضًا

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


