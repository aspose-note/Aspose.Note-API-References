---
title: Class PdfImporter
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Importing.PdfImporter sınıf. PDF biçimindeki belgelerden içerik içe aktarmak için api sağlayan sınıf. API belirtilen seçenekleri kullanarak bir dosyada veya bir akışta bulunan PDF belgesinden içe aktarmaya izin verir. İçe aktarma seçenekleri kullanılarak geçirilirPdfImportOptions .
type: docs
weight: 270
url: /tr/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

PDF biçimindeki belgelerden içerik içe aktarmak için api sağlayan sınıf. API, belirtilen seçenekleri kullanarak bir dosyada veya bir akışta bulunan PDF belgesinden içe aktarmaya izin verir. İçe aktarma seçenekleri kullanılarak geçirilir[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | Sağlanan bir akıştan PDF belgesinin içeriğini içe aktarır. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | Belirli bir dosyadan PDF belgesinin içeriğini içe aktarır. |

### Örnekler

Her 5 sayfada bir tek bir OneNote sayfasına gruplayarak PDF belgesindeki tüm sayfaların nasıl içe aktarılacağını gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

IEnumerable<Page> pages = PdfImporter.Import(Path.Combine(dataDir, "SampleGrouping.pdf"));
while (pages.Any())
{
    d.Merge(pages.Take(5), mergeOptions);
    pages = pages.Skip(5);
}

d.Save(Path.Combine(dataDir, "sample_CustomMerge.one"));
```

### Ayrıca bakınız

* ad alanı [Aspose.Note.Importing](../../aspose.note.importing/)
* toplantı [Aspose.Note](../../)


