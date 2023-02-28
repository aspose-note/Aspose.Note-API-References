---
title: Class NotebookImageSaveOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.NotebookImageSaveOptions kelas. Memungkinkan untuk menentukan opsi tambahan saat merender halaman buku catatan menjadi gambar.
type: docs
weight: 760
url: /id/net/aspose.note.saving/notebookimagesaveoptions/
---
## NotebookImageSaveOptions class

Memungkinkan untuk menentukan opsi tambahan saat merender halaman buku catatan menjadi gambar.

```csharp
public class NotebookImageSaveOptions : NotebookSaveOptions<ImageSaveOptions>
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [NotebookImageSaveOptions](notebookimagesaveoptions/)(SaveFormat) | Menginisialisasi instance baru dari`NotebookImageSaveOptions` kelas. |

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

Menunjukkan cara menyimpan buku catatan sebagai gambar dengan opsi yang ditentukan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [ImageSaveOptions](../imagesaveoptions/)
* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


