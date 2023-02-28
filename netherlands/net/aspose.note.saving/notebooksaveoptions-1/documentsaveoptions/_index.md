---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note voor .NET API-referentie
description: NotebookSaveOptions eigendom. Haalt of stelt de opslagopties in voor alle onderliggende documenten van het notitieblok.
type: docs
weight: 10
url: /nl/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Haalt of stelt de opslagopties in voor alle onderliggende documenten van het notitieblok.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* naamruimte [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* montage [Aspose.Note](../../../)


