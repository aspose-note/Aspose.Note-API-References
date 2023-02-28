---
title: Class PrintOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.PrintOptions kelas. Opsi yang digunakan untuk mencetak dokumen.
type: docs
weight: 860
url: /id/net/aspose.note.saving/printoptions/
---
## PrintOptions class

Opsi yang digunakan untuk mencetak dokumen.

```csharp
public class PrintOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [PrintOptions](printoptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | Mendapat atau menyetel nama dokumen yang akan ditampilkan (misalnya, dalam kotak dialog status cetak atau antrian printer) saat mencetak dokumen. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | Mendapatkan atau menyetel algoritme yang digunakan untuk pemisahan halaman. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | Mendapat atau mengatur pengaturan printer. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | Mendapat atau menyetel resolusi untuk gambar yang dihasilkan, dalam titik per inci. |

### Contoh

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

### Lihat juga

* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


