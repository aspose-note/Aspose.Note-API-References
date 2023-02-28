---
title: Class NotebookLoadOptions
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.NotebookLoadOptions classe. Opzioni utilizzate per caricare un taccuino.
type: docs
weight: 420
url: /it/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

Opzioni utilizzate per caricare un taccuino.

```csharp
public class NotebookLoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | Ottiene o imposta un valore che indica se i documenti secondari devono essere caricati in modo esplicito in un secondo momento. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | Ottiene o imposta un valore che indica se i documenti figlio devono essere caricati durante il caricamento del documento padre. |

### Esempi

Mostra come creare un notebook crittografato.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Guarda anche

* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


