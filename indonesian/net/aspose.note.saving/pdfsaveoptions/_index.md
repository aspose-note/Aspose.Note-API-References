---
title: Class PdfSaveOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.PdfSaveOptions kelas. Memungkinkan untuk menentukan opsi tambahan saat merender halaman dokumen ke PDF.
type: docs
weight: 850
url: /id/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Memungkinkan untuk menentukan opsi tambahan saat merender halaman dokumen ke PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Mendapatkan atau menyetel pengaturan font untuk digunakan saat menyimpan |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression/) { get; set; } | Mendapat atau menyetel jenis kompresi yang diterapkan pada gambar dalam file PDF. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality/) { get; set; } | Mendapat atau menetapkan nilai yang menentukan kualitas gambar JPEG di dalam dokumen PDF. Nilai dapat bervariasi dari 0 hingga 100 di mana 0 berarti kualitas terburuk tetapi kompresi maksimum dan 100 berarti kualitas terbaik tetapi kompresi minimum. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Mendapat atau mengatur jumlah halaman yang akan disimpan. Secara default adalahMaxValue yang berarti semua halaman dokumen akan dirender. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Mendapat atau menetapkan indeks halaman pertama yang akan disimpan. Secara default adalah 0. |
| [PageSettings](../../aspose.note.saving/pdfsaveoptions/pagesettings/) { get; set; } | Mendapat atau mengatur pengaturan halaman untuk setiap halaman dalam dokumen. Secara default tergantung pada CurrentUICulture, *Budaya AS memiliki pengaturan huruf, yang lain memiliki pengaturan A4. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/) { get; set; } | Mendapatkan atau menyetel algoritme yang digunakan untuk pemisahan halaman. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Mendapatkan format penyimpanan dokumen. |

### Contoh

Menunjukkan cara menyimpan dokumen dalam format Pdf dengan tata letak halaman Surat.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Simpan dokumen.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Menunjukkan cara menyimpan dokumen dalam format Pdf dengan tata letak halaman A4 tanpa batas ketinggian.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Simpan dokumen.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
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

Menampilkan cara menyimpan dokumen dalam format pdf.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inisialisasi objek PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Tetapkan indeks halaman dari halaman pertama yang akan disimpan
                              PageIndex = 0,

                              // Setel jumlah halaman
                              PageCount = 1,
                          };

// Simpan dokumen sebagai PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Menunjukkan cara menyimpan dokumen dalam format pdf menggunakan pengaturan khusus.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Inisialisasi objek PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Gunakan kompresi Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kualitas untuk kompresi JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions/)
* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


