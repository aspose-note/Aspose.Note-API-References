---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note untuk Referensi .NET API
description: NotebookSaveOptions Properti. Mendapat atau menyetel opsi simpan untuk semua dokumen anak buku catatan.
type: docs
weight: 10
url: /id/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Mendapat atau menyetel opsi simpan untuk semua dokumen anak buku catatan.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

### Contoh

Menunjukkan cara menyimpan buku catatan dalam format pdf dengan opsi yang ditentukan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Simpan Buku Catatan
notebook.Save(dataDir, notebookSaveOptions);
```

### Lihat juga

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* ruang nama [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* perakitan [Aspose.Note](../../../)


