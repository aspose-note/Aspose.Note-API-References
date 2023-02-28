---
title: Class KeepPartAndCloneSolidObjectToNextPageAlgorithm
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm kelas. Menambahkan bagian atas objek ke bagian bawah halaman dan mengkloning objek penuh ke halaman berikutnya jika tidak sesuai dengan halaman aslinya.
type: docs
weight: 730
url: /id/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

Menambahkan bagian atas objek ke bagian bawah halaman dan mengkloning objek penuh ke halaman berikutnya jika tidak sesuai dengan halaman aslinya.

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | Menginisialisasi instance baru dari`KeepPartAndCloneSolidObjectToNextPageAlgorithm` kelas, menggunakan batas ketinggian default dari bagian kloning. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | Menginisialisasi instance baru dari`KeepPartAndCloneSolidObjectToNextPageAlgorithm` kelas, menggunakan batas ketinggian tertentu dari bagian kloning. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | Mendapat batas tinggi dari bagian kloning. |

## Bidang

| Nama | Keterangan |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | Ukuran maksimal default dari bagian kloning. |

### Contoh

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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


