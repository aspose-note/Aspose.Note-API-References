---
title: Enum BinarizationMethod
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.BinarizationMethod Sıralama. Bir görüntü için ikili hale getirme yöntemini belirtir.
type: docs
weight: 560
url: /tr/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

Bir görüntü için ikili hale getirme yöntemini belirtir.

```csharp
public enum BinarizationMethod
```

### değerler

| İsim | Değer | Tanım |
| --- | --- | --- |
| FixedThreshold | `0` | Görüntünün ikilileştirilmesi, belirtilen sabit eşik kullanılarak gerçekleştirilir. |
| Otsu | `1` | Görüntünün ikili hale getirilmesi, eşiği değerlendirmek için Otsu'nun yöntemi kullanılarak uyarlamalı olarak gerçekleştirilir. |

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


