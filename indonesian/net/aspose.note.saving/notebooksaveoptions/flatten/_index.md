---
title: NotebookSaveOptions.Flatten
second_title: Aspose.Note untuk Referensi .NET API
description: NotebookSaveOptions Properti. Mendapat atau menyetel nilai yang menunjukkan apakah hierarki anak buku catatan disimpan secara rata.
type: docs
weight: 20
url: /id/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

Mendapat atau menyetel nilai yang menunjukkan apakah hierarki anak buku catatan disimpan secara rata.

```csharp
public bool Flatten { get; set; }
```

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

* class [NotebookSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../notebooksaveoptions/)
* perakitan [Aspose.Note](../../../)


