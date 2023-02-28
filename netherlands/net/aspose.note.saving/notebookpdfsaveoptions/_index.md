---
title: Class NotebookPdfSaveOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.NotebookPdfSaveOptions klas. Maakt het mogelijk om extra opties te specificeren bij het renderen van notebookpaginas naar PDF.
type: docs
weight: 780
url: /nl/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

Maakt het mogelijk om extra opties te specificeren bij het renderen van notebookpagina's naar PDF.

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Haalt of stelt een waarde in die aangeeft of onderliggende documenten expliciet moeten worden opgeslagen. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de onderliggende hiërarchie van het notitieblok plat wordt opgeslagen. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

### Voorbeelden

Laat zien hoe u een notitieblok in pdf-indeling kunt opslaan met opgegeven opties.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Sla het notitieblok op
notebook.Save(dataDir, notebookSaveOptions);
```

### Zie ook

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


