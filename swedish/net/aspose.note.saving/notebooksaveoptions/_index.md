---
title: Class NotebookSaveOptions
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Saving.NotebookSaveOptions klass. En abstrakt basklass som representerar anteckningsbokens sparalternativ för ett visst format.
type: docs
weight: 790
url: /sv/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

En abstrakt basklass som representerar anteckningsbokens sparalternativ för ett visst format.

```csharp
public abstract class NotebookSaveOptions
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Hämtar eller ställer in ett värde som anger om underordnade documents ska sparas explicit. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Hämtar eller ställer in ett värde som anger om anteckningsbokens barnhierarki sparas tillplattad. |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | Hämtar formatet som anteckningsboken sparas i. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | Får sparalternativen för alla anteckningsbokens underordnade dokument. |

### Exempel

Visar hur man sparar tillplattad anteckningsbok i pdf-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Spara anteckningsboken
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

Visar hur man sparar tillplattad anteckningsbok som bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Spara anteckningsboken
notebook.Save(dataDir, notebookSaveOptions);
```

### Se även

* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving/)
* hopsättning [Aspose.Note](../../)


