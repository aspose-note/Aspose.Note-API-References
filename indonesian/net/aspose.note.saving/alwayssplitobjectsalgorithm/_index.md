---
title: Class AlwaysSplitObjectsAlgorithm
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm kelas. Membagi objek menjadi beberapa bagian jika tidak sesuai dengan halaman aslinya.
type: docs
weight: 550
url: /id/net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

Membagi objek menjadi beberapa bagian jika tidak sesuai dengan halaman aslinya.

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | Konstruktor default. |

### Contoh

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


