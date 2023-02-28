---
title: Class ImageSaveOptions
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.ImageSaveOptions sınıf. Belge sayfalarını görüntülere dönüştürürken ek seçenekler belirlemeye izin verir.
type: docs
weight: 720
url: /tr/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Belge sayfalarını görüntülere dönüştürürken ek seçenekler belirlemeye izin verir.

```csharp
public class ImageSaveOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | Yeni bir örneğini başlatır.`ImageSaveOptions` sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | Görüntünün ikilileştirilmesi için seçenekleri alır veya ayarlar. |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | Alır veya ayarlar[`ColorMode`](./colormode/) çıktı görüntüsü için. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Kaydederken kullanılacak yazı tipi ayarlarını alır veya ayarlar |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Kaydedilecek sayfa sayısını alır veya ayarlar. varsayılan olarakMaxValue , bu, belgenin tüm sayfalarının oluşturulacağı anlamına gelir. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Kaydedilecek ilk sayfanın dizinini alır veya ayarlar. Varsayılan olarak 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | Kaydedilen görüntünün kalitesini belirleyen bir değer alır veya ayarlar. Bu değer codec'e System.Drawing.Imaging.Encoder.Quality parametresi olarak iletilir. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | Oluşturulan görüntülerin çözünürlüğünü inç başına nokta cinsinden alır veya ayarlar. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Belgenin kaydedildiği biçimi alır. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | Oluşturulan görüntüleri TIFF biçiminde kaydederken kullanılacak sıkıştırma türünü alır veya ayarlar. |

### Örnekler

Bir belgenin SaveFormat kullanılarak Jpeg formatında resim olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Belgeyi kaydedin.
oneFile.Save(dataDir, SaveFormat.Jpeg);
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

ImageSaveOptions kullanılarak bir belgenin Bmp biçiminde görüntü olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Belgeyi kaydedin.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Belgeyi görüntü olarak kaydederken görüntü çözünürlüğünün nasıl ayarlanacağını gösterir.

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

PackBits sıkıştırması kullanılarak bir belgenin Tiff biçiminde görüntü olarak nasıl kaydedileceğini gösterir.

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

Not defterini belirtilen seçeneklerle resim olarak nasıl kaydedeceğinizi gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Bir OneNote Not Defteri yükleyin
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Not Defterini Kaydet
notebook.Save(dataDir, notebookSaveOptions);
```

Jpeg sıkıştırması kullanılarak bir belgenin Tiff biçiminde görüntü olarak nasıl kaydedileceğini gösterir.

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

Düzleştirilmiş not defterinin resim olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Bir OneNote Not Defteri yükleyin
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Not Defterini Kaydet
notebook.Save(dataDir, notebookSaveOptions);
```

CCITT Grup 3 faks sıkıştırması kullanılarak bir belgenin Tiff biçiminde görüntü olarak nasıl kaydedileceğini gösterir.

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

Bir belgenin png formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// ImageSaveOptions nesnesini başlat 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Sayfa dizinini ayarla
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Belgeyi PNG olarak kaydedin.
oneFile.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions/)
* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


