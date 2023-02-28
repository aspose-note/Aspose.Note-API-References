---
title: Class NotebookLoadOptions
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.NotebookLoadOptions klas. Optionen zum Laden eines Notebooks.
type: docs
weight: 420
url: /de/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

Optionen zum Laden eines Notebooks.

```csharp
public class NotebookLoadOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | Ruft oder setzt einen Wert, der angibt, ob untergeordnete Dokumente explizit später geladen werden sollen. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob untergeordnete Dokumente geladen werden sollen, während das übergeordnete Dokument geladen wird. |

### Beispiele

Zeigt, wie man ein verschlüsseltes Notizbuch erstellt.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Siehe auch

* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


