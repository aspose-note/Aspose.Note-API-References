---
title: "NotebookSaveOptions.Flatten"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية NotebookSaveOptions. يحصل أو يعيّن قيمة تشير إلى ما إذا كان هيكل الأطفال في الدفتر يُحفظ مسطحًا"
type: docs
weight: 20
url: /ar/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان هيكل الأطفال في الدفتر يُحفظ مسطحًا.

```csharp
public bool Flatten { get; set; }
```

## أمثلة

يوضح كيفية حفظ الدفتر المسطح بصيغة PDF.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

// احفظ الدفتر
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

يوضح كيفية حفظ الدفتر المسطح كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// احفظ الدفتر
notebook.Save(dataDir, notebookSaveOptions);
```

### انظر أيضًا

* class [NotebookSaveOptions](../)
* namespace [Aspose.Note.Saving](../../notebooksaveoptions/)
* assembly [Aspose.Note](../../../)


