---
title: SaveFormat
second_title: Aspose.Note for .NET API Referansı
description: Belgenin kaydedildiği biçimi belirtir.
type: docs
weight: 520
url: /tr/net/aspose.note/saveformat/
---
## SaveFormat enumeration

Belgenin kaydedildiği biçimi belirtir.

```csharp
public enum SaveFormat
```

### değerler

| İsim | Değer | Tanım |
| --- | --- | --- |
| Png | `1` | Çıktının bir PNG dosyası olduğunu belirtir. |
| Bmp | `2` | Çıktının bir BMP dosyası olduğunu belirtir. |
| Jpeg | `3` | Çıktının bir JPEG dosyası olduğunu belirtir. |
| Gif | `4` | Çıktının bir GIF dosyası olduğunu belirtir. |
| Tiff | `5` | Çıktının bir TIFF dosyası olduğunu belirtir. |
| Pdf | `6` | Çıktının bir PDF dosyası olduğunu belirtir. |
| One | `7` | Çıktının bir OneNote dosyası olduğunu belirtir. |
| Html | `8` | Çıktının bir HTML dosyası olduğunu belirtir. |

### Örnekler

SaveFormat numaralandırma kullanılarak bir belgenin nasıl kaydedileceğini gösterir.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Varsayılan ayarlar kullanılarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

SaveFormat kullanılarak bir belgenin Jpeg formatında nasıl görüntü olarak kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Belgeyi kaydedin.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Bir belgenin gif biçiminde nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Belgeyi gif olarak kaydedin.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Belgeyi JPEG biçiminde görüntü olarak kaydederken görüntü kalitesinin nasıl ayarlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Belgeyi kaydedin.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

ImageSaveOptions kullanılarak bir belgenin Bmp formatında görüntü olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Belgeyi kaydedin.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Belgeyi resim olarak kaydederken bir resim çözünürlüğünün nasıl ayarlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Belgeyi kaydedin.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Bir belgenin gri tonlamalı görüntü olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Belgeyi gif olarak kaydedin.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

PackBits sıkıştırması kullanılarak bir belgenin Tiff formatında nasıl görüntü olarak kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Belgeyi kaydedin.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Jpeg sıkıştırması kullanılarak bir belgenin Tiff formatında görüntü olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Belgeyi kaydedin.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

CCITT Group 3 faks sıkıştırması kullanılarak bir belgenin Tiff formatında görüntü olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Belgeyi kaydedin.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

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

* ad alanı [Aspose.Note](../../aspose.note)
* toplantı [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
