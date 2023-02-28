---
title: Class MergeOptions
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.MergeOptions kelas. Opsi untuk menggabungkan kumpulan halaman.
type: docs
weight: 340
url: /id/net/aspose.note/mergeoptions/
---
## MergeOptions class

Opsi untuk menggabungkan kumpulan halaman.

```csharp
public class MergeOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [MergeOptions](mergeoptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah akan mengimpor halaman yang disediakan sebagai satu halaman. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah halaman yang disisipkan harus ditambahkan sebagai turunan dari halaman sebelumnya. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | Mendapat atau mengatur posisi di mana halaman yang diimpor akan disisipkan. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | Mendapat atau menyetel jarak antar halaman saat diimpor sebagai satu halaman. |

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

Memperlihatkan cara mengimpor semua halaman dari sekumpulan dokumen PDF sambil menyisipkan halaman dari setiap dokumen PDF sebagai turunan dari halaman OneNote tingkat atas.

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

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


