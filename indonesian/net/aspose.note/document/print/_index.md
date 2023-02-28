---
title: Document.Print
second_title: Aspose.Note untuk Referensi .NET API
description: Document metode. Mencetak dokumen menggunakan printer default.
type: docs
weight: 130
url: /id/net/aspose.note/document/print/
---
## Print() {#print}

Mencetak dokumen menggunakan printer default.

```csharp
public void Print()
```

### Contoh

Menunjukkan cara mengirim dokumen ke printer menggunakan dialog Windows standar dengan opsi default.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
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

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

Mencetak dokumen menggunakan printer default.

```csharp
public void Print(PrintOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| options | PrintOptions | Opsi yang digunakan untuk mencetak dokumen. Bisa null. |

### Lihat juga

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


