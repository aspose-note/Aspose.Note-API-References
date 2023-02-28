---
title: Class KeepSolidObjectsAlgorithm
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.KeepSolidObjectsAlgorithm kelas. Menggeser seluruh objek ke halaman berikutnya jika tidak sesuai dengan halaman aslinya.
type: docs
weight: 740
url: /id/net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

Menggeser seluruh objek ke halaman berikutnya jika tidak sesuai dengan halaman aslinya.

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | Menginisialisasi instance baru dari`KeepSolidObjectsAlgorithm` kelas menggunakan batas tinggi default dari bagian kloning. |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | Menginisialisasi instance baru dari`KeepSolidObjectsAlgorithm` kelas menggunakan batas ketinggian tertentu dari bagian kloning. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | Mendapat batas tinggi dari bagian kloning. |

## Bidang

| Nama | Keterangan |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | Ukuran maksimal default dari bagian kloning. |

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

Menunjukkan cara mengirim dokumen ke printer menggunakan dialog Windows standar dengan opsi yang ditentukan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


