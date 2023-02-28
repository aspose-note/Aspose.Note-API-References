---
title: Enum TiffCompression
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.TiffCompression Sıralama. Bir belgeyi TIFF biçiminde kaydederken ne tür sıkıştırma kullanılacağını belirtir.
type: docs
weight: 880
url: /tr/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

Bir belgeyi TIFF biçiminde kaydederken ne tür sıkıştırma kullanılacağını belirtir.

```csharp
public enum TiffCompression
```

### değerler

| İsim | Değer | Tanım |
| --- | --- | --- |
| None | `1` | Sıkıştırma olmadığını belirtir. |
| Rle | `2` | RLE sıkıştırmasını belirtir. |
| Ccitt3 | `3` | CCITT Grup 3 faks kodlamasını belirtir. |
| Ccitt4 | `4` | CCITT Grup 4 faks kodlamasını belirtir. |
| Lzw | `5` | LZW sıkıştırmasını belirtir. |
| PackBits | `32773` | Macintosh RLE sıkıştırmasını belirtir. |
| Jpeg | `7` | JPEG DCT sıkıştırma sıkıştırmasını belirtir. |

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

* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


