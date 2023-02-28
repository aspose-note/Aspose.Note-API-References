---
title: Class NotebookSaveOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.NotebookSaveOptions klas. Een abstracte basisklasse die opties voor het opslaan van notebooks vertegenwoordigt voor een bepaald formaat.
type: docs
weight: 790
url: /nl/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

Een abstracte basisklasse die opties voor het opslaan van notebooks vertegenwoordigt voor een bepaald formaat.

```csharp
public abstract class NotebookSaveOptions
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Haalt of stelt een waarde in die aangeeft of onderliggende documenten expliciet moeten worden opgeslagen. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de onderliggende hiërarchie van het notitieblok plat wordt opgeslagen. |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | Haalt de indeling op waarin het notitieboek is opgeslagen. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | Krijgt de opslagopties voor alle onderliggende documenten van het notitieblok. |

### Voorbeelden

Laat zien hoe u een afgeplat notitieboek in pdf-formaat kunt opslaan.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Sla het notitieblok op
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

Laat zien hoe u een afgeplat notitieboek als afbeelding kunt opslaan.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Sla het notitieblok op
notebook.Save(dataDir, notebookSaveOptions);
```

### Zie ook

* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


