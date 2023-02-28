---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note untuk Referensi .NET API
description: PdfSaveOptions Properti. Mendapat atau menetapkan nilai yang menentukan kualitas gambar JPEG di dalam dokumen PDF. Nilai dapat bervariasi dari 0 hingga 100 di mana 0 berarti kualitas terburuk tetapi kompresi maksimum dan 100 berarti kualitas terbaik tetapi kompresi minimum.
type: docs
weight: 30
url: /id/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

Mendapat atau menetapkan nilai yang menentukan kualitas gambar JPEG di dalam dokumen PDF. Nilai dapat bervariasi dari 0 hingga 100 di mana 0 berarti kualitas terburuk tetapi kompresi maksimum dan 100 berarti kualitas terbaik tetapi kompresi minimum.

```csharp
public int JpegQuality { get; set; }
```

### Perkataan

Nilai standarnya adalah 90.

### Contoh

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

### Lihat juga

* class [PdfSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../pdfsaveoptions/)
* perakitan [Aspose.Note](../../../)


