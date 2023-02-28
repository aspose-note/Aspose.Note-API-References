---
title: ImageSaveOptions.Resolution
second_title: Aspose.Note untuk Referensi .NET API
description: ImageSaveOptions Properti. Mendapat atau menyetel resolusi untuk gambar yang dihasilkan dalam titik per inci.
type: docs
weight: 50
url: /id/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

Mendapat atau menyetel resolusi untuk gambar yang dihasilkan, dalam titik per inci.

```csharp
public float Resolution { get; set; }
```

### Perkataan

Nilai standarnya adalah 96.

### Contoh

Menunjukkan cara menyetel resolusi gambar saat menyimpan dokumen sebagai gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Simpan dokumen.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
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

* class [ImageSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../imagesaveoptions/)
* perakitan [Aspose.Note](../../../)


