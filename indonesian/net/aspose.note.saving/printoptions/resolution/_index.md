---
title: PrintOptions.Resolution
second_title: Aspose.Note untuk Referensi .NET API
description: PrintOptions Properti. Mendapat atau menyetel resolusi untuk gambar yang dihasilkan dalam titik per inci.
type: docs
weight: 50
url: /id/net/aspose.note.saving/printoptions/resolution/
---
## PrintOptions.Resolution property

Mendapat atau menyetel resolusi untuk gambar yang dihasilkan, dalam titik per inci.

```csharp
public float Resolution { get; set; }
```

### Perkataan

Nilai standarnya adalah 96.

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


