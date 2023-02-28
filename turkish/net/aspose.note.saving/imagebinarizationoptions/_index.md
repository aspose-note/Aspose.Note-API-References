---
title: Class ImageBinarizationOptions
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.ImageBinarizationOptions sınıf. Görüntünün ikili hale getirilmesi için seçenekler.
type: docs
weight: 710
url: /tr/net/aspose.note.saving/imagebinarizationoptions/
---
## ImageBinarizationOptions class

Görüntünün ikili hale getirilmesi için seçenekler.

```csharp
public class ImageBinarizationOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [ImageBinarizationOptions](imagebinarizationoptions/)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BinarizationMethod](../../aspose.note.saving/imagebinarizationoptions/binarizationmethod/) { get; set; } | Binarizasyon yöntemini alır veya ayarlar. Varsayılan değer:FixedThreshold . |
| [BinarizationThreshold](../../aspose.note.saving/imagebinarizationoptions/binarizationthreshold/) { get; set; } | Sabit eşik ikilileştirme yöntemi için eşik değeri alır veya ayarlar. Varsayılan değer 128. 'dir. |

### Örnekler

Otsu'nun yöntemini kullanarak bir belgenin ikili görüntü olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Belgeyi gif olarak kaydedin.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Sabit eşik kullanılarak bir belgenin ikili görüntü olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Belgeyi gif olarak kaydedin.
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

### Ayrıca bakınız

* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


