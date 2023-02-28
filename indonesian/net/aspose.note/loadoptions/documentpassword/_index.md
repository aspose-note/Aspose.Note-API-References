---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note untuk Referensi .NET API
description: LoadOptions Properti. Mendapat atau menyetel kata sandi untuk konten dokumen terenkripsi. Nilai diabaikan jika dokumen tidak dilindungi kata sandi.
type: docs
weight: 20
url: /id/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

Mendapat atau menyetel kata sandi untuk konten dokumen terenkripsi. Nilai diabaikan jika dokumen tidak dilindungi kata sandi.

```csharp
public string DocumentPassword { get; set; }
```

### Contoh

Menunjukkan bagaimana sebuah dokumen terenkripsi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Menunjukkan cara membuat buku catatan terenkripsi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Lihat juga

* class [LoadOptions](../)
* ruang nama [Aspose.Note](../../loadoptions/)
* perakitan [Aspose.Note](../../../)


