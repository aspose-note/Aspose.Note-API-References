---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note voor .NET API-referentie
description: NotebookLoadOptions eigendom. Haalt of stelt een waarde in die aangeeft of onderliggende documenten expliciet later moeten worden geladen.
type: docs
weight: 20
url: /nl/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

Haalt of stelt een waarde in die aangeeft of onderliggende documenten expliciet later moeten worden geladen.

```csharp
public bool DeferredLoading { get; set; }
```

### Opmerkingen

Standaardwaarde is`vals` , dus onderliggende documenten worden impliciet geladen. Waarde`WAAR` geeft aan dat de gebruiker moet bellen[`LoadChildDocument`](../../notebook/loadchilddocument/) of voor het onderliggende knooppunt van elke notebook nadat de notebook zelf is geladen. Als de waarde is`WAAR` ,[`InstantLoading`](../instantloading/) optie wordt genegeerd. Als notebook wordt geladen vanuit stream, is de waarde altijd`WAAR` ondanks was expliciet door de gebruiker ingesteld op`vals` .

### Voorbeelden

Laat zien hoe je een versleuteld notitieboekje gebruikt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Zie ook

* class [NotebookLoadOptions](../)
* naamruimte [Aspose.Note](../../notebookloadoptions/)
* montage [Aspose.Note](../../../)


