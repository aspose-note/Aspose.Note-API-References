---
title: SaveOptions.PageCount
second_title: Aspose.Note for .NET API Referansı
description: SaveOptions mülk. Kaydedilecek sayfa sayısını alır veya ayarlar. varsayılan olarakMaxValue  bu belgenin tüm sayfalarının oluşturulacağı anlamına gelir.
type: docs
weight: 20
url: /tr/net/aspose.note.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Kaydedilecek sayfa sayısını alır veya ayarlar. varsayılan olarakMaxValue , bu, belgenin tüm sayfalarının oluşturulacağı anlamına gelir.

```csharp
public int PageCount { get; set; }
```

### Örnekler

Bir belgenin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions nesnesini başlat
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Kaydedilecek ilk sayfanın sayfa dizinini ayarla
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
                              // Jpeg sıkıştırmayı kullan
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG sıkıştırma kalitesi
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Bir belgenin nasıl oluşturulacağını ve belirtilen sayfa aralığında html formatında kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote belgesini başlat
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Belgedeki tüm metin için varsayılan stil.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML formatında kaydet
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

### Ayrıca bakınız

* class [SaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../saveoptions/)
* toplantı [Aspose.Note](../../../)


