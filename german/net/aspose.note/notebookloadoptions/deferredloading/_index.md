---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note für .NET-API-Referenz
description: NotebookLoadOptions eigendom. Ruft oder setzt einen Wert der angibt ob untergeordnete Dokumente explizit später geladen werden sollen.
type: docs
weight: 20
url: /de/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

Ruft oder setzt einen Wert, der angibt, ob untergeordnete Dokumente explizit später geladen werden sollen.

```csharp
public bool DeferredLoading { get; set; }
```

### Bemerkungen

Standardwert ist`FALSCH` , sodass untergeordnete Dokumente implizit geladen werden. Wert`WAHR` zeigt an, dass der Benutzer anrufen soll[`LoadChildDocument`](../../notebook/loadchilddocument/) oder für den untergeordneten Knoten jedes Notebooks, nachdem das Notebook selbst geladen wurde. Wenn der Wert ist`WAHR` ,[`InstantLoading`](../instantloading/) Die Option wird ignoriert. Wenn das Notebook vom Stream geladen wird, ist der Wert immer`WAHR` obwohl vom Benutzer explizit auf gesetzt wurde`FALSCH` .

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

* class [NotebookLoadOptions](../)
* namensraum [Aspose.Note](../../notebookloadoptions/)
* Montage [Aspose.Note](../../../)


