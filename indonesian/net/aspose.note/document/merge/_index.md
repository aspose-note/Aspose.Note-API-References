---
title: Document.Merge
second_title: Aspose.Note untuk Referensi .NET API
description: Document metode. Menggabungkan satu set halaman ke dokumen.
type: docs
weight: 120
url: /id/net/aspose.note/document/merge/
---
## Document.Merge method

Menggabungkan satu set halaman ke dokumen.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pages | IEnumerable`1 | Kumpulan halaman. |
| mergeOptions | MergeOptions | Menentukan opsi cara menggabungkan halaman yang disediakan. |

### Nilai Pengembalian

Mengembalikan referensi ke dokumen.

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

### Lihat juga

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


