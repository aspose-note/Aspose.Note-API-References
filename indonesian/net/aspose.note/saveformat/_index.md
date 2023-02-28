---
title: Enum SaveFormat
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.SaveFormat enum. Menunjukkan format penyimpanan dokumen.
type: docs
weight: 540
url: /id/net/aspose.note/saveformat/
---
## SaveFormat enumeration

Menunjukkan format penyimpanan dokumen.

```csharp
public enum SaveFormat
```

### Nilai

| Nama | Nilai | Keterangan |
| --- | --- | --- |
| Png | `1` | Menentukan bahwa keluarannya adalah file PNG. |
| Bmp | `2` | Menentukan bahwa output adalah file BMP. |
| Jpeg | `3` | Menentukan bahwa output adalah file JPEG. |
| Gif | `4` | Menentukan bahwa output adalah file GIF. |
| Tiff | `5` | Menentukan bahwa output adalah file TIFF. |
| Pdf | `6` | Menentukan bahwa output adalah file PDF. |
| One | `7` | Menentukan bahwa output adalah file OneNote. |
| Html | `8` | Menentukan bahwa output adalah file HTML. |

### Contoh

Menunjukkan cara menyimpan dokumen menggunakan pencacahan SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

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

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


