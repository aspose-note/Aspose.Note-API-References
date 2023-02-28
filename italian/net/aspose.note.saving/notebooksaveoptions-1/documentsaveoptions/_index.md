---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note per .NET API Reference
description: NotebookSaveOptions proprietà. Ottiene o imposta le opzioni di salvataggio per tutti i documenti secondari del notebook.
type: docs
weight: 10
url: /it/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Ottiene o imposta le opzioni di salvataggio per tutti i documenti secondari del notebook.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

### Esempi

Mostra come salvare il notebook in formato pdf con le opzioni specificate.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Carica un blocco appunti di OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Salva il taccuino
notebook.Save(dataDir, notebookSaveOptions);
```

### Guarda anche

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* spazio dei nomi [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* assemblea [Aspose.Note](../../../)


