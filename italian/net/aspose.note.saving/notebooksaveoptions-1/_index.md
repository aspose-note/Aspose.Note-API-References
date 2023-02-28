---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions classe. Una classe di base astratta che rappresenta le opzioni di salvataggio del notebook per un particolare formato e fornisce opzioni di salvataggio comuni per tutti i nodi figlio del documento.
type: docs
weight: 800
url: /it/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

Una classe di base astratta che rappresenta le opzioni di salvataggio del notebook per un particolare formato e fornisce opzioni di salvataggio comuni per tutti i nodi figlio del documento.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| Parametro | Descrizione |
| --- | --- |
| TDocumentSaveOptions | Le opzioni di salvataggio per tutti i documenti secondari del taccuino. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Ottiene o imposta un valore che indica se i documenti secondari devono essere salvati in modo esplicito. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | Ottiene o imposta le opzioni di salvataggio per tutti i documenti secondari del notebook. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Ottiene o imposta un valore che indica se la gerarchia degli elementi secondari del blocco appunti viene salvata in modalità flat. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | Ottiene il formato in cui viene salvato il notebook. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | Ottiene le opzioni di salvataggio per tutti i documenti secondari del blocco appunti. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* spazio dei nomi [Aspose.Note.Saving](../../aspose.note.saving/)
* assemblea [Aspose.Note](../../)


