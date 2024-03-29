---
title: NotebookSaveOptions.Flatten
second_title: Aspose.Note for .NET API Reference
description: NotebookSaveOptions property. Gets or sets a value indicating whether the notebook children hierarchy is saved flattened
type: docs
weight: 20
url: /net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

Gets or sets a value indicating whether the notebook children hierarchy is saved flattened.

```csharp
public bool Flatten { get; set; }
```

## Examples

Shows how to save flattened notebook in pdf format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Save the Notebook
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Shows how to save flattened notebook as image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Save the Notebook
notebook.Save(dataDir, notebookSaveOptions);
```

### See Also

* class [NotebookSaveOptions](../)
* namespace [Aspose.Note.Saving](../../notebooksaveoptions/)
* assembly [Aspose.Note](../../../)


