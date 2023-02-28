---
title: ImageSaveOptions.Quality
second_title: Aspose.Note for .NET API Referansı
description: ImageSaveOptions mülk. Kaydedilen görüntünün kalitesini belirleyen bir değer alır veya ayarlar. Bu değer codece System.Drawing.Imaging.Encoder.Quality parametresi olarak iletilir.
type: docs
weight: 40
url: /tr/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

Kaydedilen görüntünün kalitesini belirleyen bir değer alır veya ayarlar. Bu değer codec'e System.Drawing.Imaging.Encoder.Quality parametresi olarak iletilir.

```csharp
public int Quality { get; set; }
```

### Notlar

Kalite kategorisi için faydalı değer aralığı 0 ile 100 arasındadır. Belirtilen sayı ne kadar düşükse, sıkıştırma o kadar yüksek olur ve bu nedenle görüntünün kalitesi o kadar düşük olur. Sıfır size en düşük kaliteli görüntüyü ve 100 en yüksek görüntüyü verir . Varsayılan değer 90. 'dir.

### Örnekler

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

### Ayrıca bakınız

* class [ImageSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../imagesaveoptions/)
* toplantı [Aspose.Note](../../../)


