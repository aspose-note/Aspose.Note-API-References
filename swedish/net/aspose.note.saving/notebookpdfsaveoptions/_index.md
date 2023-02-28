---
title: Class NotebookPdfSaveOptions
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Saving.NotebookPdfSaveOptions klass. Gör det möjligt att ange ytterligare alternativ när du renderar anteckningsboksidor till PDF.
type: docs
weight: 780
url: /sv/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

Gör det möjligt att ange ytterligare alternativ när du renderar anteckningsboksidor till PDF.

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Hämtar eller ställer in ett värde som anger om underordnade documents ska sparas explicit. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Hämtar eller ställer in ett värde som anger om anteckningsbokens barnhierarki sparas tillplattad. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving/)
* hopsättning [Aspose.Note](../../)


