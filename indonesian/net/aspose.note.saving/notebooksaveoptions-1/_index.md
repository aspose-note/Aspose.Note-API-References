---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions kelas. Kelas dasar abstrak yang mewakili opsi penyimpanan notebook untuk format tertentu dan menyediakan opsi penyimpanan umum untuk semua node anak dokumen.
type: docs
weight: 800
url: /id/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

Kelas dasar abstrak yang mewakili opsi penyimpanan notebook untuk format tertentu dan menyediakan opsi penyimpanan umum untuk semua node anak dokumen.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| Parameter | Keterangan |
| --- | --- |
| TDocumentSaveOptions | Opsi simpan untuk semua dokumen anak buku catatan. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah dokumen turunan harus disimpan secara eksplisit. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | Mendapat atau menyetel opsi simpan untuk semua dokumen anak buku catatan. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Mendapat atau menyetel nilai yang menunjukkan apakah hierarki anak buku catatan disimpan secara rata. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | Mendapatkan format penyimpanan buku catatan. |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | Mendapatkan opsi simpan untuk semua dokumen anak buku catatan. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


