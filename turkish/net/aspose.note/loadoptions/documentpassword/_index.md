---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note for .NET API Referansı
description: LoadOptions mülk. Şifrelenmiş belge içeriği için bir parola alır veya ayarlar. Belgenin parola korumalı olmaması durumunda değer dikkate alınmaz.
type: docs
weight: 20
url: /tr/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

Şifrelenmiş belge içeriği için bir parola alır veya ayarlar. Belgenin parola korumalı olmaması durumunda değer dikkate alınmaz.

```csharp
public string DocumentPassword { get; set; }
```

### Örnekler

Bir belgenin nasıl şifreleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Not defterinin nasıl şifreleneceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Ayrıca bakınız

* class [LoadOptions](../)
* ad alanı [Aspose.Note](../../loadoptions/)
* toplantı [Aspose.Note](../../../)


