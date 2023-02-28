---
title: ImageSaveOptions.Resolution
second_title: Aspose.Note för .NET API-referens
description: ImageSaveOptions fast egendom. Hämtar eller ställer in upplösningen för de genererade bilderna i punkter per tum.
type: docs
weight: 50
url: /sv/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

Hämtar eller ställer in upplösningen för de genererade bilderna, i punkter per tum.

```csharp
public float Resolution { get; set; }
```

### Anmärkningar

Standardvärdet är 96.

### Exempel

Visar hur du ställer in en bildupplösning när du sparar dokument som bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Spara dokumentet.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Visar hur du sparar anteckningsboken som bild med angivna alternativ.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Ladda en OneNote-anteckningsbok
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

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

* class [ImageSaveOptions](../)
* namnutrymme [Aspose.Note.Saving](../../imagesaveoptions/)
* hopsättning [Aspose.Note](../../../)


