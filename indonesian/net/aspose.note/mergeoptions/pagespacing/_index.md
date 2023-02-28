---
title: MergeOptions.PageSpacing
second_title: Aspose.Note untuk Referensi .NET API
description: MergeOptions Properti. Mendapat atau menyetel jarak antar halaman saat diimpor sebagai satu halaman.
type: docs
weight: 50
url: /id/net/aspose.note/mergeoptions/pagespacing/
---
## MergeOptions.PageSpacing property

Mendapat atau menyetel jarak antar halaman saat diimpor sebagai satu halaman.

```csharp
public float PageSpacing { get; set; }
```

### Contoh

Memperlihatkan cara mengimpor semua halaman dari pengelompokan dokumen PDF setiap 5 halaman ke satu halaman OneNote.

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

Memperlihatkan cara mengimpor semua konten dari sekumpulan dokumen PDF sambil menggabungkan halaman dari setiap dokumen PDF ke satu halaman OneNote.

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

### Lihat juga

* class [MergeOptions](../)
* ruang nama [Aspose.Note](../../mergeoptions/)
* perakitan [Aspose.Note](../../../)


