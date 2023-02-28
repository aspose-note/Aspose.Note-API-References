---
title: ImageSaveOptions.TiffCompression
second_title: Aspose.Note untuk Referensi .NET API
description: ImageSaveOptions Properti. Mendapatkan atau menyetel jenis kompresi yang akan digunakan saat menyimpan gambar yang dihasilkan ke format TIFF.
type: docs
weight: 60
url: /id/net/aspose.note.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Mendapatkan atau menyetel jenis kompresi yang akan digunakan saat menyimpan gambar yang dihasilkan ke format TIFF.

```csharp
public TiffCompression TiffCompression { get; set; }
```

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

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../imagesaveoptions/)
* perakitan [Aspose.Note](../../../)


