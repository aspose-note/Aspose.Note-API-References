---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note for .NET API Reference
description: NotebookSaveOptions property. Gets or sets the save options for all notebooks child documents
type: docs
weight: 10
url: /net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Gets or sets the save options for all notebook's child documents.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

## Examples

Shows how to save notebook in pdf format with specified options.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Save the Notebook
notebook.Save(dataDir, notebookSaveOptions);
```

### See Also

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* namespace [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* assembly [Aspose.Note](../../../)


