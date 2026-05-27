---
title: "الفئة NotebookSaveOptionsTDocumentSaveOptions"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions. فئة أساسية مجردة تمثل خيارات حفظ الدفتر لتنسيق معين وتوفر خيارات حفظ مشتركة لجميع عقد المستند الفرعية"
type: docs
weight: 880
url: /ar/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

فئة أساسية مجردة تمثل خيارات حفظ الدفتر لتنسيق معين وتوفر خيارات حفظ مشتركة لجميع العقد الفرعية للمستند.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| معامل | الوصف |
| --- | --- |
| TDocumentSaveOptions | خيارات الحفظ لجميع المستندات الفرعية للدفتر. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب حفظ المستندات الفرعية صراحةً. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | يحصل أو يعيّن خيارات الحفظ لجميع المستندات الفرعية للدفتر. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان هيكل الأطفال في الدفتر يُحفظ مسطحًا. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | يحصل على الصيغة التي يُحفظ بها الدفتر. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | يحصل على خيارات الحفظ لجميع المستندات الفرعية للدفتر. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


