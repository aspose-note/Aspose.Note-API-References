---
title: Document.Save
second_title: Aspose.Note untuk Referensi .NET API
description: Document metode. Menyimpan dokumen OneNote ke file.
type: docs
weight: 140
url: /id/net/aspose.note/document/save/
---
## Save(string) {#save_3}

Menyimpan dokumen OneNote ke file.

```csharp
public void Save(string fileName)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileName | String | Nama lengkap file. Jika file dengan nama lengkap yang ditentukan sudah ada, file yang ada akan ditimpa. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Struktur dokumen melanggar spesifikasi. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Format penyimpanan yang diminta tidak didukung. |

### Contoh

Menunjukkan cara menyimpan dokumen.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Menyimpan dokumen OneNote ke aliran.

```csharp
public void Save(Stream stream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | System.IO.Stream tempat dokumen akan disimpan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Struktur dokumen melanggar spesifikasi. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Format penyimpanan yang diminta tidak didukung. |

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Menyimpan dokumen OneNote ke file dalam format yang ditentukan.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileName | String | Nama lengkap file. Jika file dengan nama lengkap yang ditentukan sudah ada, file yang ada akan ditimpa. |
| format | SaveFormat | Format untuk menyimpan dokumen. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Struktur dokumen melanggar spesifikasi. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Format penyimpanan yang diminta tidak didukung. |

### Contoh

Menunjukkan cara menyimpan dokumen menggunakan pencacahan SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Menunjukkan cara menyimpan dokumen dalam format gif.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Simpan dokumen sebagai gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

### Lihat juga

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Menyimpan dokumen OneNote ke aliran dalam format yang ditentukan.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | System.IO.Stream tempat dokumen akan disimpan. |
| format | SaveFormat | Format untuk menyimpan dokumen. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Struktur dokumen melanggar spesifikasi. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Format penyimpanan yang diminta tidak didukung. |

### Contoh

Menunjukkan cara menyimpan dokumen dalam format pdf menggunakan pengaturan default.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Simpan dokumen sebagai PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Menunjukkan cara menyimpan dokumen ke aliran.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Putar ulang posisi aliran kembali ke nol sehingga siap untuk pembaca berikutnya.
dstStream.Seek(0, SeekOrigin.Begin);
```

Menunjukkan cara menerapkan gaya tema Gelap ke Dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### Lihat juga

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Menyimpan dokumen OneNote ke file menggunakan opsi penyimpanan yang ditentukan.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileName | String | Nama lengkap file. Jika file dengan nama lengkap yang ditentukan sudah ada, file yang ada akan ditimpa. |
| options | SaveOptions | Menentukan opsi bagaimana dokumen disimpan dalam file. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Struktur dokumen melanggar spesifikasi. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Format penyimpanan yang diminta tidak didukung. |

### Contoh

Menunjukkan cara menyimpan dokumen menggunakan OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Menunjukkan cara menyimpan dokumen sebagai gambar dalam format Jpeg menggunakan SaveFormat.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Simpan dokumen.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Menunjukkan cara menyimpan dokumen sebagai gambar dalam format Bmp menggunakan ImageSaveOptions.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Simpan dokumen.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Menunjukkan cara menyimpan dokumen dalam format Pdf dengan tata letak halaman Surat.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Simpan dokumen.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Menunjukkan cara menyimpan dokumen dalam format Pdf dengan tata letak halaman A4 tanpa batas ketinggian.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Simpan dokumen.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

Menunjukkan cara menyimpan dokumen sebagai gambar skala abu-abu.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Simpan dokumen sebagai gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Menunjukkan cara menyimpan dokumen sebagai gambar dalam format Tiff menggunakan kompresi PackBits.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Simpan dokumen.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Menunjukkan cara menyimpan dokumen sebagai gambar dalam format Tiff menggunakan kompresi Jpeg.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Simpan dokumen.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Menunjukkan cara menyimpan dokumen sebagai gambar dalam format Tiff menggunakan kompresi faks CCITT Group 3.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Simpan dokumen.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

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

Menunjukkan cara menyimpan dokumen sebagai citra biner menggunakan metode Otsu.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Simpan dokumen sebagai gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Menunjukkan cara menyimpan dokumen sebagai gambar biner menggunakan ambang tetap.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Simpan dokumen sebagai gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### Lihat juga

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Menyimpan dokumen OneNote ke aliran menggunakan opsi penyimpanan yang ditentukan.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | System.IO.Stream tempat dokumen akan disimpan. |
| options | SaveOptions | Menentukan opsi bagaimana dokumen disimpan dalam aliran. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Struktur dokumen melanggar spesifikasi. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Format penyimpanan yang diminta tidak didukung. |

### Contoh

Menunjukkan cara menyimpan dokumen dalam format pdf menggunakan font default yang ditentukan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Simpan dokumen sebagai PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Menunjukkan cara menyimpan dokumen dalam format pdf menggunakan font default dari file.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Simpan dokumen sebagai PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Menunjukkan cara menyimpan dokumen dalam format pdf menggunakan font default dari aliran.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Simpan dokumen sebagai PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Lihat juga

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


