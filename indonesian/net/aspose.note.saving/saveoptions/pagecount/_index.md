---
title: SaveOptions.PageCount
second_title: Aspose.Note untuk Referensi .NET API
description: SaveOptions Properti. Mendapat atau mengatur jumlah halaman yang akan disimpan. Secara default adalahMaxValue yang berarti semua halaman dokumen akan dirender.
type: docs
weight: 20
url: /id/net/aspose.note.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Mendapat atau mengatur jumlah halaman yang akan disimpan. Secara default adalahMaxValue yang berarti semua halaman dokumen akan dirender.

```csharp
public int PageCount { get; set; }
```

### Contoh

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

Menunjukkan cara membuat dokumen dan menyimpan dalam format html rentang halaman yang ditentukan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Inisialisasi dokumen OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Gaya default untuk semua teks dalam dokumen.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Simpan ke dalam format HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

### Lihat juga

* class [SaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../saveoptions/)
* perakitan [Aspose.Note](../../../)


