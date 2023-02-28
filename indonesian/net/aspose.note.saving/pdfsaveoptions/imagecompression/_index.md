---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note untuk Referensi .NET API
description: PdfSaveOptions Properti. Mendapat atau menyetel jenis kompresi yang diterapkan pada gambar dalam file PDF.
type: docs
weight: 20
url: /id/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

Mendapat atau menyetel jenis kompresi yang diterapkan pada gambar dalam file PDF.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

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

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../pdfsaveoptions/)
* perakitan [Aspose.Note](../../../)


