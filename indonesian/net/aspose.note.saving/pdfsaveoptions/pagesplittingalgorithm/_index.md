---
title: PdfSaveOptions.PageSplittingAlgorithm
second_title: Aspose.Note untuk Referensi .NET API
description: PdfSaveOptions Properti. Mendapatkan atau menyetel algoritme yang digunakan untuk pemisahan halaman.
type: docs
weight: 50
url: /id/net/aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/
---
## PdfSaveOptions.PageSplittingAlgorithm property

Mendapatkan atau menyetel algoritme yang digunakan untuk pemisahan halaman.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### Nilai properti

Itu`PageSplittingAlgorithm` .

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

Saat halaman OneNote yang panjang disimpan dalam format pdf, halaman tersebut dibagi menjadi beberapa halaman. Contoh menunjukkan cara mengonfigurasi logika pemisahan objek yang terletak di hentian halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// atau
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Saat halaman OneNote yang panjang disimpan dalam format pdf, halaman tersebut dibagi menjadi beberapa halaman. Contoh menunjukkan cara mengonfigurasi logika pemisahan objek yang terletak di hentian halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Atau
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Atau
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Atau
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Atau
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Lihat juga

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PdfSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../pdfsaveoptions/)
* perakitan [Aspose.Note](../../../)


