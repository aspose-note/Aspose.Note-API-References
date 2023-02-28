---
title: Document.Import
second_title: Aspose.Note for .NET API Referansı
description: Document yöntem. Sağlanan PDF belgesinden bir dizi sayfayı içe aktarır.
type: docs
weight: 110
url: /tr/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

Sağlanan PDF belgesinden bir dizi sayfayı içe aktarır.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | PDF belgeli bir akış. |
| importOptions | PdfImportOptions | Sayfaların PDF belgesinden nasıl içe aktarılacağını belirtir. |
| mergeOptions | MergeOptions | Sağlanan sayfaların nasıl birleştirileceğini belirtir. |

### Geri dönüş değeri

Belgeye yapılan başvuruyu döndürür.

### Ayrıca bakınız

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

Sağlanan PDF belgesinden bir dizi sayfayı içe aktarır.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| file | String | PDF belgesi içeren bir dosya. |
| importOptions | PdfImportOptions | Sayfaların PDF belgesinden nasıl içe aktarılacağını belirtir. |
| mergeOptions | MergeOptions | Sağlanan sayfaların nasıl birleştirileceğini belirtir. |

### Geri dönüş değeri

Belgeye yapılan başvuruyu döndürür.

### Örnekler

Bir dizi PDF belgesinden tüm sayfaların sayfa sayfa nasıl içe aktarılacağını gösterir.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)


