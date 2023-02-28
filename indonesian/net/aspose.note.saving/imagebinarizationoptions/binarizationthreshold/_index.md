---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note untuk Referensi .NET API
description: ImageBinarizationOptions Properti. Mendapat atau menetapkan nilai ambang untuk metode binarisasi ambang tetap. Nilai defaultnya adalah 128.
type: docs
weight: 30
url: /id/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

Mendapat atau menetapkan nilai ambang untuk metode binarisasi ambang tetap. Nilai defaultnya adalah 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

### Contoh

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

* class [ImageBinarizationOptions](../)
* ruang nama [Aspose.Note.Saving](../../imagebinarizationoptions/)
* perakitan [Aspose.Note](../../../)


