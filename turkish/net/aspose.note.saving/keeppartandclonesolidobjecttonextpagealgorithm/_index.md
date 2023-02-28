---
title: Class KeepPartAndCloneSolidObjectToNextPageAlgorithm
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm sınıf. Nesnenin üst kısmını sayfanın altına ekler ve orijinal sayfaya sığmaması durumunda tüm nesneyi bir sonraki sayfaya kopyalar.
type: docs
weight: 730
url: /tr/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

Nesnenin üst kısmını sayfanın altına ekler ve orijinal sayfaya sığmaması durumunda tüm nesneyi bir sonraki sayfaya kopyalar.

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | Yeni bir örneğini başlatır.`KeepPartAndCloneSolidObjectToNextPageAlgorithm` sınıf, klonlanmış parçanın varsayılan yükseklik sınırını kullanıyor. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | Yeni bir örneğini başlatır.`KeepPartAndCloneSolidObjectToNextPageAlgorithm` sınıf, klonlanmış parçanın belirli yükseklik sınırını kullanarak. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | Klonlanan parçanın yükseklik sınırını alır. |

## Alanlar

| İsim | Tanım |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | Klonlanan parçanın varsayılan maksimum boyutu. |

### Örnekler

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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


