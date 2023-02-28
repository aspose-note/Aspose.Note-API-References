---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note för .NET API-referens
description: NotebookLoadOptions fast egendom. Hämtar eller ställer in ett värde som anger om underordnade documents ska laddas explicit senare.
type: docs
weight: 20
url: /sv/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

Hämtar eller ställer in ett värde som anger om underordnade documents ska laddas explicit senare.

```csharp
public bool DeferredLoading { get; set; }
```

### Anmärkningar

Standardvärdet är`falsk` , så underordnade dokument kommer att laddas implicit. Value`Sann` indikerar att användaren ska ringa[`LoadChildDocument`](../../notebook/loadchilddocument/) eller för varje anteckningsboks underordnade nod efter att själva anteckningsboken har laddats. Om värdet är`Sann` ,[`InstantLoading`](../instantloading/) alternativet kommer att ignoreras. Om notebook-datorn laddas från stream är värdet alltid`Sann` trots ställdes uttryckligen av användaren till`falsk` .

### Exempel

Visar hur man använder en krypterad anteckningsbok.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Se även

* class [NotebookLoadOptions](../)
* namnutrymme [Aspose.Note](../../notebookloadoptions/)
* hopsättning [Aspose.Note](../../../)


