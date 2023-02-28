---
title: MergeOptions.InsertAsChild
second_title: Aspose.Note untuk Referensi .NET API
description: MergeOptions Properti. Mendapat atau menetapkan nilai yang menunjukkan apakah halaman yang disisipkan harus ditambahkan sebagai turunan dari halaman sebelumnya.
type: docs
weight: 30
url: /id/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

Mendapat atau menetapkan nilai yang menunjukkan apakah halaman yang disisipkan harus ditambahkan sebagai turunan dari halaman sebelumnya.

```csharp
public bool InsertAsChild { get; set; }
```

### Contoh

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

### Lihat juga

* class [MergeOptions](../)
* ruang nama [Aspose.Note](../../mergeoptions/)
* perakitan [Aspose.Note](../../../)


