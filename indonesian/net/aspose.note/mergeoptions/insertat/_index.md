---
title: MergeOptions.InsertAt
second_title: Aspose.Note untuk Referensi .NET API
description: MergeOptions Properti. Mendapat atau mengatur posisi di mana halaman yang diimpor akan disisipkan.
type: docs
weight: 40
url: /id/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

Mendapat atau mengatur posisi di mana halaman yang diimpor akan disisipkan.

```csharp
public int InsertAt { get; set; }
```

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException |  |

### Perkataan

Jika nilainya lebih besar dari jumlah halaman dalam dokumen target, maka halaman yang diimpor ditambahkan ke bagian akhir dokumen.

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


