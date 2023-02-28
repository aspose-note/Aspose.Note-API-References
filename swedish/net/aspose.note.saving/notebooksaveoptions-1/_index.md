---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions klass. En abstrakt basklass som representerar anteckningsbokens sparalternativ för ett visst format och ger gemensamma sparalternativ för alla underordnade dokumentnoder.
type: docs
weight: 800
url: /sv/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

En abstrakt basklass som representerar anteckningsbokens sparalternativ för ett visst format och ger gemensamma sparalternativ för alla underordnade dokumentnoder.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| Parameter | Beskrivning |
| --- | --- |
| TDocumentSaveOptions | Spara alternativen för alla anteckningsbokens underordnade dokument. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Hämtar eller ställer in ett värde som anger om underordnade documents ska sparas explicit. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | Hämtar eller ställer in sparalternativ för alla anteckningsbokens underordnade dokument. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Hämtar eller ställer in ett värde som anger om anteckningsbokens barnhierarki sparas tillplattad. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | Hämtar formatet som anteckningsboken sparas i. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | Får sparalternativen för alla anteckningsbokens underordnade dokument. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving/)
* hopsättning [Aspose.Note](../../)


