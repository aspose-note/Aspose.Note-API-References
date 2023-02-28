---
title: Enum TiffCompression
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.TiffCompression enum. Menentukan jenis kompresi yang akan digunakan saat menyimpan dokumen ke format TIFF.
type: docs
weight: 880
url: /id/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

Menentukan jenis kompresi yang akan digunakan saat menyimpan dokumen ke format TIFF.

```csharp
public enum TiffCompression
```

### Nilai

| Nama | Nilai | Keterangan |
| --- | --- | --- |
| None | `1` | Menentukan tanpa kompresi. |
| Rle | `2` | Menentukan kompresi RLE. |
| Ccitt3 | `3` | Menentukan penyandian faks CCITT Grup 3. |
| Ccitt4 | `4` | Menentukan penyandian faks CCITT Grup 4. |
| Lzw | `5` | Menentukan kompresi LZW. |
| PackBits | `32773` | Menentukan kompresi RLE Macintosh. |
| Jpeg | `7` | Menentukan kompresi kompresi JPEG DCT. |

### Contoh

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

### Lihat juga

* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


