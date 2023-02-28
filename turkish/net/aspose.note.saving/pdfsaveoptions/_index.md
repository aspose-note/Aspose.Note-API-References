---
title: Class PdfSaveOptions
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.PdfSaveOptions sınıf. Belge sayfalarını PDFye dönüştürürken ek seçenekler belirlemeye izin verir.
type: docs
weight: 850
url: /tr/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Belge sayfalarını PDF'ye dönüştürürken ek seçenekler belirlemeye izin verir.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Kaydederken kullanılacak yazı tipi ayarlarını alır veya ayarlar |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression/) { get; set; } | PDF dosyasındaki görüntülere uygulanan sıkıştırma türünü alır veya ayarlar. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality/) { get; set; } | PDF belgesindeki JPEG görüntülerinin kalitesini belirleyen bir değer alır veya ayarlar. Değer 0 ile 100 arasında değişebilir; burada 0, en kötü kalite ancak maksimum sıkıştırma anlamına gelir ve 100, en iyi kalite ancak minimum sıkıştırma anlamına gelir. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Kaydedilecek sayfa sayısını alır veya ayarlar. varsayılan olarakMaxValue , bu, belgenin tüm sayfalarının oluşturulacağı anlamına gelir. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Kaydedilecek ilk sayfanın dizinini alır veya ayarlar. Varsayılan olarak 0. |
| [PageSettings](../../aspose.note.saving/pdfsaveoptions/pagesettings/) { get; set; } | Belgedeki her sayfa için sayfa ayarlarını alır veya ayarlar. Varsayılan olarak CurrentUICulture'a bağlıdır, *ABD kültürlerinin harf ayarı vardır, diğerlerinin A4 ayarları vardır. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm/) { get; set; } | Sayfa bölme için kullanılan algoritmayı alır veya ayarlar. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Belgenin kaydedildiği biçimi alır. |

### Örnekler

Bir belgenin Letter sayfa düzeniyle PDF formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Belgeyi kaydedin.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Bir belgenin A4 sayfa düzeninde yükseklik sınırı olmaksızın PDF formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Belgeyi kaydedin.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

Not defterinin belirtilen seçeneklerle pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Bir OneNote Not Defteri yükleyin
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Not Defterini Kaydet
notebook.Save(dataDir, notebookSaveOptions);
```

Uzun OneNote sayfaları pdf biçiminde kaydedildiğinde, sayfalar arasında bölünürler. Örnek, sayfa sonlarında bulunan nesnelerin bölme mantığının nasıl yapılandırılacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
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

Uzun OneNote sayfaları pdf biçiminde kaydedildiğinde, sayfalar arasında bölünürler. Örnek, sayfa sonlarında bulunan nesnelerin bölme mantığının nasıl yapılandırılacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Veya
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Ayrıca bakınız

* class [SaveOptions](../saveoptions/)
* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


