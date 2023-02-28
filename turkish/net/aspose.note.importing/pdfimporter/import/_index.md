---
title: PdfImporter.Import
second_title: Aspose.Note for .NET API Referansı
description: PdfImporter yöntem. Sağlanan bir akıştan PDF belgesinin içeriğini içe aktarır.
type: docs
weight: 10
url: /tr/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

Sağlanan bir akıştan PDF belgesinin içeriğini içe aktarır.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Akış. |
| options | PdfImportOptions | Seçenekler. |

### Geri dönüş değeri

[`PdfImporter`](../) .

### Ayrıca bakınız

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* ad alanı [Aspose.Note.Importing](../../pdfimporter/)
* toplantı [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

Belirli bir dosyadan PDF belgesinin içeriğini içe aktarır.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| file | String | PDF dosyası. |
| options | PdfImportOptions | Seçenekler. |

### Geri dönüş değeri

[`PdfImporter`](../) .

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* ad alanı [Aspose.Note.Importing](../../pdfimporter/)
* toplantı [Aspose.Note](../../../)


