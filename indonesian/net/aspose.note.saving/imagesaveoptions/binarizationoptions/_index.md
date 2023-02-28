---
title: ImageSaveOptions.BinarizationOptions
second_title: Aspose.Note untuk Referensi .NET API
description: ImageSaveOptions Properti. Mendapat atau menyetel opsi untuk binarisasi gambar.
type: docs
weight: 20
url: /id/net/aspose.note.saving/imagesaveoptions/binarizationoptions/
---
## ImageSaveOptions.BinarizationOptions property

Mendapat atau menyetel opsi untuk binarisasi gambar.

```csharp
public ImageBinarizationOptions BinarizationOptions { get; set; }
```

### Contoh

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

* class [ImageBinarizationOptions](../../imagebinarizationoptions/)
* class [ImageSaveOptions](../)
* ruang nama [Aspose.Note.Saving](../../imagesaveoptions/)
* perakitan [Aspose.Note](../../../)


