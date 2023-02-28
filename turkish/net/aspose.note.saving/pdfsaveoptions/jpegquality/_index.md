---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note for .NET API Referansı
description: PdfSaveOptions mülk. PDF belgesindeki JPEG görüntülerinin kalitesini belirleyen bir değer alır veya ayarlar. Değer 0 ile 100 arasında değişebilir burada 0 en kötü kalite ancak maksimum sıkıştırma anlamına gelir ve 100 en iyi kalite ancak minimum sıkıştırma anlamına gelir.
type: docs
weight: 30
url: /tr/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

PDF belgesindeki JPEG görüntülerinin kalitesini belirleyen bir değer alır veya ayarlar. Değer 0 ile 100 arasında değişebilir; burada 0, en kötü kalite ancak maksimum sıkıştırma anlamına gelir ve 100, en iyi kalite ancak minimum sıkıştırma anlamına gelir.

```csharp
public int JpegQuality { get; set; }
```

### Notlar

Varsayılan değer 90. 'dir.

### Örnekler

Belirli ayarlar kullanılarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions nesnesini başlat
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Jpeg sıkıştırmayı kullan
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG sıkıştırma kalitesi
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

### Ayrıca bakınız

* class [PdfSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../pdfsaveoptions/)
* toplantı [Aspose.Note](../../../)


