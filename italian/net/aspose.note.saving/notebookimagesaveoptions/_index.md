---
title: Class NotebookImageSaveOptions
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Saving.NotebookImageSaveOptions classe. Consente di specificare opzioni aggiuntive durante il rendering delle pagine del taccuino in immagini.
type: docs
weight: 760
url: /it/net/aspose.note.saving/notebookimagesaveoptions/
---
## NotebookImageSaveOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del taccuino in immagini.

```csharp
public class NotebookImageSaveOptions : NotebookSaveOptions<ImageSaveOptions>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [NotebookImageSaveOptions](notebookimagesaveoptions/)(SaveFormat) | Inizializza una nuova istanza di`NotebookImageSaveOptions` classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Ottiene o imposta un valore che indica se i documenti secondari devono essere salvati in modo esplicito. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Ottiene o imposta un valore che indica se la gerarchia degli elementi secondari del blocco appunti viene salvata in modalità flat. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

### Esempi

Mostra come salvare il taccuino appiattito in formato pdf.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Salva il taccuino
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [ImageSaveOptions](../imagesaveoptions/)
* spazio dei nomi [Aspose.Note.Saving](../../aspose.note.saving/)
* assemblea [Aspose.Note](../../)


