---
title: MergeOptions.InsertAt
second_title: Aspose.Note for .NET API Referansı
description: MergeOptions mülk. İçe aktarılan sayfaların ekleneceği konumu alır veya ayarlar.
type: docs
weight: 40
url: /tr/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

İçe aktarılan sayfaların ekleneceği konumu alır veya ayarlar.

```csharp
public int InsertAt { get; set; }
```

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException |  |

### Notlar

Değer, hedef belgedeki sayfa sayısından büyükse, içe aktarılan sayfalar belgenin sonuna eklenir.

### Örnekler

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

### Ayrıca bakınız

* class [MergeOptions](../)
* ad alanı [Aspose.Note](../../mergeoptions/)
* toplantı [Aspose.Note](../../../)


