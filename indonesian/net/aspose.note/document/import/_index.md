---
title: Document.Import
second_title: Aspose.Note untuk Referensi .NET API
description: Document metode. Mengimpor sekumpulan halaman dari dokumen PDF yang disediakan.
type: docs
weight: 110
url: /id/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

Mengimpor sekumpulan halaman dari dokumen PDF yang disediakan.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Aliran dengan dokumen PDF. |
| importOptions | PdfImportOptions | Menentukan opsi cara mengimpor halaman dari dokumen PDF. |
| mergeOptions | MergeOptions | Menentukan opsi cara menggabungkan halaman yang disediakan. |

### Nilai Pengembalian

Mengembalikan referensi ke dokumen.

### Lihat juga

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

Mengimpor sekumpulan halaman dari dokumen PDF yang disediakan.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| file | String | File dengan dokumen PDF. |
| importOptions | PdfImportOptions | Menentukan opsi cara mengimpor halaman dari dokumen PDF. |
| mergeOptions | MergeOptions | Menentukan opsi cara menggabungkan halaman yang disediakan. |

### Nilai Pengembalian

Mengembalikan referensi ke dokumen.

### Contoh

Menunjukkan cara mengimpor semua halaman dari sekumpulan dokumen PDF halaman demi halaman.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


