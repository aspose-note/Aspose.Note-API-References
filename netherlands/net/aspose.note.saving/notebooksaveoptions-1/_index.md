---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions klas. Een abstracte basisklasse die notebookopslagopties vertegenwoordigt voor een bepaald formaat en gemeenschappelijke opslagopties biedt voor alle onderliggende documentknooppunten.
type: docs
weight: 800
url: /nl/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

Een abstracte basisklasse die notebook-opslagopties vertegenwoordigt voor een bepaald formaat en gemeenschappelijke opslagopties biedt voor alle onderliggende documentknooppunten.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| Parameter | Beschrijving |
| --- | --- |
| TDocumentSaveOptions | De opslagopties voor alle onderliggende documenten van het notitieblok. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Haalt of stelt een waarde in die aangeeft of onderliggende documenten expliciet moeten worden opgeslagen. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | Haalt of stelt de opslagopties in voor alle onderliggende documenten van het notitieblok. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de onderliggende hiërarchie van het notitieblok plat wordt opgeslagen. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | Haalt de indeling op waarin het notitieboek is opgeslagen. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | Krijgt de opslagopties voor alle onderliggende documenten van het notitieblok. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


