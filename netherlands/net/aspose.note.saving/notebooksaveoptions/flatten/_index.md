---
title: NotebookSaveOptions.Flatten
second_title: Aspose.Note voor .NET API-referentie
description: NotebookSaveOptions eigendom. Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de onderliggende hiërarchie van het notitieblok plat wordt opgeslagen.
type: docs
weight: 20
url: /nl/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de onderliggende hiërarchie van het notitieblok plat wordt opgeslagen.

```csharp
public bool Flatten { get; set; }
```

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

* class [NotebookSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../notebooksaveoptions/)
* montage [Aspose.Note](../../../)


