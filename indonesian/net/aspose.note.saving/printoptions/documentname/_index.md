---
title: PrintOptions.DocumentName
second_title: Aspose.Note untuk Referensi .NET API
description: PrintOptions Properti. Mendapat atau menyetel nama dokumen yang akan ditampilkan misalnya dalam kotak dialog status cetak atau antrian printer saat mencetak dokumen.
type: docs
weight: 20
url: /id/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

Mendapat atau menyetel nama dokumen yang akan ditampilkan (misalnya, dalam kotak dialog status cetak atau antrian printer) saat mencetak dokumen.

```csharp
public string DocumentName { get; set; }
```

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

* class [PrintOptions](../)
* ruang nama [Aspose.Note.Saving](../../printoptions/)
* perakitan [Aspose.Note](../../../)


