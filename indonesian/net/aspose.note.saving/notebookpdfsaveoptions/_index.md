---
title: Class NotebookPdfSaveOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.NotebookPdfSaveOptions kelas. Memungkinkan untuk menentukan opsi tambahan saat merender halaman buku catatan ke PDF.
type: docs
weight: 780
url: /id/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

Memungkinkan untuk menentukan opsi tambahan saat merender halaman buku catatan ke PDF.

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah dokumen turunan harus disimpan secara eksplisit. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Mendapat atau menyetel nilai yang menunjukkan apakah hierarki anak buku catatan disimpan secara rata. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## Metode

| Nama | Keterangan |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


