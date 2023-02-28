---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note för .NET API-referens
description: NotebookSaveOptions fast egendom. Hämtar eller ställer in sparalternativ för alla anteckningsbokens underordnade dokument.
type: docs
weight: 10
url: /sv/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Hämtar eller ställer in sparalternativ för alla anteckningsbokens underordnade dokument.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

### Exempel

Visar hur du sparar anteckningsboken i pdf-format med angivna alternativ.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Spara anteckningsboken
notebook.Save(dataDir, notebookSaveOptions);
```

### Se även

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* namnutrymme [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* hopsättning [Aspose.Note](../../../)


