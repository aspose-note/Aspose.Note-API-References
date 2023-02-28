---
title: ImageSaveOptions.Resolution
second_title: Aspose.Note voor .NET API-referentie
description: ImageSaveOptions eigendom. Hiermee wordt de resolutie voor de gegenereerde afbeeldingen opgehaald of ingesteld in dots per inch.
type: docs
weight: 50
url: /nl/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

Hiermee wordt de resolutie voor de gegenereerde afbeeldingen opgehaald of ingesteld, in dots per inch.

```csharp
public float Resolution { get; set; }
```

### Opmerkingen

De standaardwaarde is 96.

### Voorbeelden

Laat zien hoe u een afbeeldingsresolutie instelt bij het opslaan van een document als afbeelding.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Sla het document op.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Laat zien hoe u een notitieblok kunt opslaan als afbeelding met opgegeven opties.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Laad een OneNote-notitieblok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

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

* class [ImageSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../imagesaveoptions/)
* montage [Aspose.Note](../../../)


