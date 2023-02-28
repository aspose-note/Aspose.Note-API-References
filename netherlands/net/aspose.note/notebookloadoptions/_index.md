---
title: Class NotebookLoadOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.NotebookLoadOptions klas. Opties gebruikt om een notebook te laden.
type: docs
weight: 420
url: /nl/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

Opties gebruikt om een notebook te laden.

```csharp
public class NotebookLoadOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | Haalt of stelt een waarde in die aangeeft of onderliggende documenten expliciet later moeten worden geladen. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | Haalt of stelt een waarde in die aangeeft of onderliggende documenten moeten worden geladen terwijl het bovenliggende document wordt geladen. |

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

* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


