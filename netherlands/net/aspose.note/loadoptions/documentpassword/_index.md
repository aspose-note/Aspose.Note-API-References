---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note voor .NET API-referentie
description: LoadOptions eigendom. Haalt of stelt een wachtwoord in voor de versleutelde documentinhoud. Waarde wordt genegeerd als het document niet met een wachtwoord is beveiligd.
type: docs
weight: 20
url: /nl/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

Haalt of stelt een wachtwoord in voor de versleutelde documentinhoud. Waarde wordt genegeerd als het document niet met een wachtwoord is beveiligd.

```csharp
public string DocumentPassword { get; set; }
```

### Voorbeelden

Laat zien hoe u een gecodeerd document maakt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

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

* class [LoadOptions](../)
* naamruimte [Aspose.Note](../../loadoptions/)
* montage [Aspose.Note](../../../)


