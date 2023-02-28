---
title: Document.Merge
second_title: Aspose.Note for .NET API Referansı
description: Document yöntem. Bir dizi sayfayı belgeyle birleştirir.
type: docs
weight: 120
url: /tr/net/aspose.note/document/merge/
---
## Document.Merge method

Bir dizi sayfayı belgeyle birleştirir.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pages | IEnumerable`1 | Bir dizi sayfa. |
| mergeOptions | MergeOptions | Sağlanan sayfaların nasıl birleştirileceğini belirtir. |

### Geri dönüş değeri

Belgeye yapılan başvuruyu döndürür.

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

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)


