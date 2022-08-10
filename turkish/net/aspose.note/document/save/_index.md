---
title: Save
second_title: Aspose.Note for .NET API Referansı
description: OneNote belgesini bir dosyaya kaydeder.
type: docs
weight: 140
url: /tr/net/aspose.note/document/save/
---
## Save(string) {#save_3}

OneNote belgesini bir dosyaya kaydeder.

```csharp
public void Save(string fileName)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | Dosyanın tam adı. Belirtilen tam ada sahip bir dosya zaten varsa, mevcut dosyanın üzerine yazılır. |

### istisnalar

| istisna | şart |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Belge yapısı belirtimi ihlal ediyor. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | İstenen kaydetme biçimi desteklenmiyor. |

### Örnekler

Bir belgenin nasıl kaydedileceğini gösterir.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Ayrıca bakınız

* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## Save(Stream) {#save}

OneNote belgesini bir akışa kaydeder.

```csharp
public void Save(Stream stream)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Belgenin kaydedileceği System.IO.Stream. |

### istisnalar

| istisna | şart |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Belge yapısı belirtimi ihlal ediyor. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | İstenen kaydetme biçimi desteklenmiyor. |

### Ayrıca bakınız

* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

OneNote belgesini belirtilen biçimde bir dosyaya kaydeder.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | Dosyanın tam adı. Belirtilen tam ada sahip bir dosya zaten varsa, mevcut dosyanın üzerine yazılır. |
| format | SaveFormat | Belgenin kaydedileceği biçim. |

### istisnalar

| istisna | şart |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Belge yapısı belirtimi ihlal ediyor. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | İstenen kaydetme biçimi desteklenmiyor. |

### Örnekler

SaveFormat numaralandırma kullanılarak bir belgenin nasıl kaydedileceğini gösterir.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
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

### Ayrıca bakınız

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

OneNote belgesini belirtilen biçimde bir akışa kaydeder.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Belgenin kaydedileceği System.IO.Stream. |
| format | SaveFormat | Belgenin kaydedileceği biçim. |

### istisnalar

| istisna | şart |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Belge yapısı belirtimi ihlal ediyor. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | İstenen kaydetme biçimi desteklenmiyor. |

### Örnekler

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

Bir belgenin akışa nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Bir sonraki okuyucu için hazır olması için akış konumunu sıfıra geri sarın.
dstStream.Seek(0, SeekOrigin.Begin);
```

### Ayrıca bakınız

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Belirtilen kaydetme seçeneklerini kullanarak OneNote belgesini bir dosyaya kaydeder.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fileName | String | Dosyanın tam adı. Belirtilen tam ada sahip bir dosya zaten varsa, mevcut dosyanın üzerine yazılır. |
| options | SaveOptions | Belgenin dosyaya nasıl kaydedileceği seçeneklerini belirtir. |

### istisnalar

| istisna | şart |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Belge yapısı belirtimi ihlal ediyor. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | İstenen kaydetme biçimi desteklenmiyor. |

### Örnekler

OneSaveOptions kullanılarak bir belgenin nasıl kaydedileceğini gösterir.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
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

Bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions nesnesini başlat
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Kaydedilecek ilk sayfanın sayfa indeksini ayarla
                              PageIndex = 0,

                              // Sayfa sayısını ayarla
                              PageCount = 1,
                          };

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Belirli ayarlar kullanılarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions nesnesini başlat
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Jpeg sıkıştırmasını kullan
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG sıkıştırması için kalite
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Belirtilen kaydetme seçeneklerini kullanarak OneNote belgesini bir akışa kaydeder.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Belgenin kaydedileceği System.IO.Stream. |
| options | SaveOptions | Belgenin akışa nasıl kaydedileceği seçeneklerini belirtir. |

### istisnalar

| istisna | şart |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | Belge yapısı belirtimi ihlal ediyor. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | İstenen kaydetme biçimi desteklenmiyor. |

### Örnekler

Belirtilen varsayılan yazı tipini kullanarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Bir dosyadan varsayılan yazı tipini kullanarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Bir akıştan varsayılan yazı tipini kullanarak bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Belgeyi PDF olarak kaydet
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Ayrıca bakınız

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* ad alanı [Aspose.Note](../../document)
* toplantı [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
