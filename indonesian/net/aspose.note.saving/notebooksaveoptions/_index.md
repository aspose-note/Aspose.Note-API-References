---
title: Class NotebookSaveOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.NotebookSaveOptions kelas. Kelas dasar abstrak yang mewakili opsi penyimpanan buku catatan untuk format tertentu.
type: docs
weight: 790
url: /id/net/aspose.note.saving/notebooksaveoptions/
---
## NotebookSaveOptions class

Kelas dasar abstrak yang mewakili opsi penyimpanan buku catatan untuk format tertentu.

```csharp
public abstract class NotebookSaveOptions
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah dokumen turunan harus disimpan secara eksplisit. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Mendapat atau menyetel nilai yang menunjukkan apakah hierarki anak buku catatan disimpan secara rata. |
| abstract [SaveFormat](../../aspose.note.saving/notebooksaveoptions/saveformat/) { get; } | Mendapatkan format penyimpanan buku catatan. |

## Metode

| Nama | Keterangan |
| --- | --- |
| abstract [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions/getdocumentsaveoptions/)() | Mendapatkan opsi simpan untuk semua dokumen anak buku catatan. |

### Contoh

Menunjukkan cara menyimpan buku catatan yang diratakan dalam format pdf.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Simpan Buku Catatan
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

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

Menunjukkan cara menyimpan buku catatan yang diratakan sebagai gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Simpan Buku Catatan
notebook.Save(dataDir, notebookSaveOptions);
```

### Lihat juga

* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


