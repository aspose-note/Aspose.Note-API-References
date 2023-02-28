---
title: Enum BinarizationMethod
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Saving.BinarizationMethod enum. Menentukan metode binarisasi untuk sebuah gambar.
type: docs
weight: 560
url: /id/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

Menentukan metode binarisasi untuk sebuah gambar.

```csharp
public enum BinarizationMethod
```

### Nilai

| Nama | Nilai | Keterangan |
| --- | --- | --- |
| FixedThreshold | `0` | Binarisasi gambar dilakukan menggunakan ambang batas tetap yang ditentukan. |
| Otsu | `1` | Binarisasi gambar dilakukan secara adaptif menggunakan metode Otsu untuk mengevaluasi threshold. |

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

* ruang nama [Aspose.Note.Saving](../../aspose.note.saving/)
* perakitan [Aspose.Note](../../)


