---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note for .NET API Reference
description: NotebookLoadOptions property. Gets or sets a value indicating whether children documents should be loaded explicitly later
type: docs
weight: 20
url: /net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

Gets or sets a value indicating whether children documents should be loaded explicitly later.

```csharp
public bool DeferredLoading { get; set; }
```

## Remarks

Default value is `false`, so child documents will be loaded implicitly. Value `true` is indicating that user should call [`LoadChildDocument`](../../notebook/loadchilddocument/) or  for each notebook's child node after notebook itself is loaded. If value is `true`, [`InstantLoading`](../instantloading/) option will be ignored. If notebook is loading from stream, the value is always `true` despite was explicitly set by user to `false`.

## Examples

Shows how to an encrypted notebook.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### See Also

* class [NotebookLoadOptions](../)
* namespace [Aspose.Note](../../notebookloadoptions/)
* assembly [Aspose.Note](../../../)


