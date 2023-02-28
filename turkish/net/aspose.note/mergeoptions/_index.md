---
title: Class MergeOptions
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.MergeOptions sınıf. Bir sayfa koleksiyonunu birleştirme seçenekleri.
type: docs
weight: 340
url: /tr/net/aspose.note/mergeoptions/
---
## MergeOptions class

Bir sayfa koleksiyonunu birleştirme seçenekleri.

```csharp
public class MergeOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [MergeOptions](mergeoptions/)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | Sağlanan sayfaların tek sayfa olarak içe aktarılıp aktarılmayacağını belirten bir değer alır veya ayarlar. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | Girilen sayfaların bir önceki sayfanın çocukları olarak eklenip eklenmeyeceğini belirten bir değer alır veya ayarlar. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | İçe aktarılan sayfaların ekleneceği konumu alır veya ayarlar. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | Tek bir sayfa olarak içe aktarıldığında sayfalar arasındaki boşluğu alır veya ayarlar. |

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

Bir üst düzey OneNote sayfasının alt öğeleri olarak her PDF belgesinden sayfalar eklerken bir dizi PDF belgesinden tüm sayfaların nasıl içe aktarılacağını gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

foreach (var file in new[] { "sampleText.pdf", "sampleImage.pdf", "sampleTable.pdf" })
{
    d.AppendChildLast(new Page()).Title = new Title() { TitleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append(file) };
    d.Import(Path.Combine(dataDir, file), new PdfImportOptions(), new MergeOptions() { InsertAt = int.MaxValue, InsertAsChild = true });
}

d.Save(Path.Combine(dataDir, "sample_StructuredMerge.one"));
```

Her PDF belgesindeki sayfaları tek bir OneNote sayfasında birleştirirken bir dizi PDF belgesinden tüm içeriğin nasıl içe aktarılacağını gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var importOptions = new PdfImportOptions();
var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

d.Import(Path.Combine(dataDir, "sampleText.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleImage.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleTable.pdf"), importOptions, mergeOptions);

d.Save(Path.Combine(dataDir, "sample_SinglePageMerge.one"));
```

### Ayrıca bakınız

* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


