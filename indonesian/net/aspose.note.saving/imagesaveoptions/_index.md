---
title: Class ImageSaveOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.ImageSaveOptions kelas. Memungkinkan untuk menentukan opsi tambahan saat merender halaman dokumen menjadi gambar.
type: docs
weight: 720
url: /id/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Memungkinkan untuk menentukan opsi tambahan saat merender halaman dokumen menjadi gambar.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | Menginisialisasi instance baru dari`ImageSaveOptions` kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | Mendapat atau menyetel opsi untuk binarisasi gambar. |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | Mendapat atau set[`ColorMode`](./colormode/) untuk gambar keluaran. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Mendapatkan atau menyetel pengaturan font untuk digunakan saat menyimpan |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Mendapat atau mengatur jumlah halaman yang akan disimpan. Secara default adalahMaxValue yang berarti semua halaman dokumen akan dirender. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Mendapat atau menetapkan indeks halaman pertama yang akan disimpan. Secara default adalah 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | Mendapat atau menetapkan nilai yang menentukan kualitas gambar yang disimpan. Nilai ini diteruskan ke codec sebagai parameter System.Drawing.Imaging.Encoder.Quality. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | Mendapat atau menyetel resolusi untuk gambar yang dihasilkan, dalam titik per inci. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Mendapatkan format penyimpanan dokumen. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | Mendapatkan atau menyetel jenis kompresi yang akan digunakan saat menyimpan gambar yang dihasilkan ke format TIFF. |

### Contoh

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

Menunjukkan cara menyetel kualitas gambar saat menyimpan dokumen sebagai gambar dalam format JPEG.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Simpan dokumen.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
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

Menunjukkan cara menyetel resolusi gambar saat menyimpan dokumen sebagai gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Simpan dokumen.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
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

Menunjukkan cara menyimpan buku catatan sebagai gambar dengan opsi yang ditentukan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Simpan Buku Catatan
notebook.Save(dataDir, notebookSaveOptions);
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

Menunjukkan cara menyimpan buku catatan yang diratakan sebagai gambar.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Simpan Buku Catatan
notebook.Save(dataDir, notebookSaveOptions);
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

Menunjukkan cara menyimpan dokumen dalam format png.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Inisialisasi objek ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Tetapkan indeks halaman
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Simpan dokumen sebagai PNG.
oneFile.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions/)
* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


