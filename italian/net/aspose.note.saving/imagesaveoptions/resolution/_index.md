---
title: ImageSaveOptions.Resolution
second_title: Aspose.Note per .NET API Reference
description: ImageSaveOptions proprietà. Ottiene o imposta la risoluzione per le immagini generate in punti per pollice.
type: docs
weight: 50
url: /it/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

Ottiene o imposta la risoluzione per le immagini generate, in punti per pollice.

```csharp
public float Resolution { get; set; }
```

### Osservazioni

Il valore predefinito è 96.

### Esempi

Mostra come impostare una risoluzione dell'immagine quando si salva il documento come immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Salva il documento.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Mostra come salvare il notebook come immagine con le opzioni specificate.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Salva il taccuino
notebook.Save(dataDir, notebookSaveOptions);
```

Mostra come salvare il taccuino appiattito come immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Salva il taccuino
notebook.Save(dataDir, notebookSaveOptions);
```

### Guarda anche

* class [ImageSaveOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../imagesaveoptions/)
* assemblea [Aspose.Note](../../../)


