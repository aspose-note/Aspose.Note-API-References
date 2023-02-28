---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note untuk Referensi .NET API
description: NotebookLoadOptions Properti. Mendapat atau menetapkan nilai yang menunjukkan apakah dokumen turunan harus dimuat secara eksplisit nanti.
type: docs
weight: 20
url: /id/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

Mendapat atau menetapkan nilai yang menunjukkan apakah dokumen turunan harus dimuat secara eksplisit nanti.

```csharp
public bool DeferredLoading { get; set; }
```

### Perkataan

Nilai defaultnya adalah`PALSU` , jadi dokumen turunan akan dimuat secara implisit. Nilai`BENAR` menunjukkan bahwa pengguna harus menelepon[`LoadChildDocument`](../../notebook/loadchilddocument/) atau untuk setiap node anak notebook setelah notebook itu sendiri dimuat. Jika nilainya`BENAR` ,[`InstantLoading`](../instantloading/) opsi akan diabaikan. Jika notebook memuat dari aliran, nilainya selalu`BENAR` meskipun secara eksplisit diatur oleh pengguna ke`PALSU` .

### Contoh

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

* class [NotebookLoadOptions](../)
* ruang nama [Aspose.Note](../../notebookloadoptions/)
* perakitan [Aspose.Note](../../../)


