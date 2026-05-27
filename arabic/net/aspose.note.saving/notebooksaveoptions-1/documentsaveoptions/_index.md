---
title: "NotebookSaveOptions1.DocumentSaveOptions"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "NotebookSaveOptions property. يحصل أو يعيّن خيارات الحفظ لجميع المستندات الفرعية للدفاتر"
type: docs
weight: 10
url: /ar/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

يحصل أو يعيّن خيارات الحفظ لجميع المستندات الفرعية للدفتر.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* namespace [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* assembly [Aspose.Note](../../../)


