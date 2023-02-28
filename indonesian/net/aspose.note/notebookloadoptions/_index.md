---
title: Class NotebookLoadOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.NotebookLoadOptions kelas. Opsi yang digunakan untuk memuat notebook.
type: docs
weight: 420
url: /id/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

Opsi yang digunakan untuk memuat notebook.

```csharp
public class NotebookLoadOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah dokumen turunan harus dimuat secara eksplisit nanti. |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah dokumen turunan harus dimuat saat dokumen induk sedang dimuat. |

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

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


