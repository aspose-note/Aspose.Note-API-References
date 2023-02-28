---
title: MergeOptions.InsertAsChild
second_title: Aspose.Note for .NET API Referansı
description: MergeOptions mülk. Girilen sayfaların bir önceki sayfanın çocukları olarak eklenip eklenmeyeceğini belirten bir değer alır veya ayarlar.
type: docs
weight: 30
url: /tr/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

Girilen sayfaların bir önceki sayfanın çocukları olarak eklenip eklenmeyeceğini belirten bir değer alır veya ayarlar.

```csharp
public bool InsertAsChild { get; set; }
```

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


