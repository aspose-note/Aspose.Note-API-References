---
title: MergeOptions.ImportAsSinglePage
second_title: Aspose.Note untuk Referensi .NET API
description: MergeOptions Properti. Mendapat atau menetapkan nilai yang menunjukkan apakah akan mengimpor halaman yang disediakan sebagai satu halaman.
type: docs
weight: 20
url: /id/net/aspose.note/mergeoptions/importassinglepage/
---
## MergeOptions.ImportAsSinglePage property

Mendapat atau menetapkan nilai yang menunjukkan apakah akan mengimpor halaman yang disediakan sebagai satu halaman.

```csharp
public bool ImportAsSinglePage { get; set; }
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


