---
title: Class NotebookPdfSaveOptions
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Saving.NotebookPdfSaveOptions classe. Consente di specificare opzioni aggiuntive durante il rendering delle pagine del taccuino in PDF.
type: docs
weight: 780
url: /it/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del taccuino in PDF.

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | Default_Costruttore |

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* spazio dei nomi [Aspose.Note.Saving](../../aspose.note.saving/)
* assemblea [Aspose.Note](../../)


