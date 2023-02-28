---
title: ImageSaveOptions.TiffCompression
second_title: Aspose.Note for .NET API Referansı
description: ImageSaveOptions mülk. Oluşturulan görüntüleri TIFF biçiminde kaydederken kullanılacak sıkıştırma türünü alır veya ayarlar.
type: docs
weight: 60
url: /tr/net/aspose.note.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Oluşturulan görüntüleri TIFF biçiminde kaydederken kullanılacak sıkıştırma türünü alır veya ayarlar.

```csharp
public TiffCompression TiffCompression { get; set; }
```

### Örnekler

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

### Ayrıca bakınız

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../imagesaveoptions/)
* toplantı [Aspose.Note](../../../)


