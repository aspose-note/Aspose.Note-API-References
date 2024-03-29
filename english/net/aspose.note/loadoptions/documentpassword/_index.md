---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note for .NET API Reference
description: LoadOptions property. Gets or sets a password for the encrypted document content. Value is ignored in case the document is not password protected
type: docs
weight: 20
url: /net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

Gets or sets a password for the encrypted document content. Value is ignored in case the document is not password protected.

```csharp
public string DocumentPassword { get; set; }
```

## Examples

Shows how to an encrypted document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

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

* class [LoadOptions](../)
* namespace [Aspose.Note](../../loadoptions/)
* assembly [Aspose.Note](../../../)


