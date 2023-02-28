---
title: ImageSaveOptions.Quality
second_title: Aspose.Note untuk Referensi .NET API
description: ImageSaveOptions Properti. Mendapat atau menetapkan nilai yang menentukan kualitas gambar yang disimpan. Nilai ini diteruskan ke codec sebagai parameter System.Drawing.Imaging.Encoder.Quality.
type: docs
weight: 40
url: /id/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

Mendapat atau menetapkan nilai yang menentukan kualitas gambar yang disimpan. Nilai ini diteruskan ke codec sebagai parameter System.Drawing.Imaging.Encoder.Quality.

```csharp
public int Quality { get; set; }
```

### Perkataan

Kisaran nilai yang berguna untuk kategori kualitas adalah dari 0 hingga 100. Semakin rendah angka yang ditentukan, semakin tinggi kompresi dan oleh karena itu semakin rendah kualitas gambar. Nol akan memberi Anda kualitas gambar terendah dan 100 tertinggi . Nilai standarnya adalah 90.

### Contoh

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

### Lihat juga

* class [ImageSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../imagesaveoptions/)
* perakitan [Aspose.Note](../../../)


