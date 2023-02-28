---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note för .NET API-referens
description: LoadOptions fast egendom. Hämtar eller ställer in ett lösenord för det krypterade dokumentinnehållet. Värdet ignoreras om dokumentet inte är lösenordsskyddat.
type: docs
weight: 20
url: /sv/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

Hämtar eller ställer in ett lösenord för det krypterade dokumentinnehållet. Värdet ignoreras om dokumentet inte är lösenordsskyddat.

```csharp
public string DocumentPassword { get; set; }
```

### Exempel

Visar hur man gör ett krypterat dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

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

* class [LoadOptions](../)
* namnutrymme [Aspose.Note](../../loadoptions/)
* hopsättning [Aspose.Note](../../../)


