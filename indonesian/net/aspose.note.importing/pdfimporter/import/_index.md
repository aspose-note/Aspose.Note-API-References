---
title: PdfImporter.Import
second_title: Aspose.Note untuk Referensi .NET API
description: PdfImporter metode. Mengimpor konten dokumen PDF dari aliran yang disediakan.
type: docs
weight: 10
url: /id/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

Mengimpor konten dokumen PDF dari aliran yang disediakan.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Arus. |
| options | PdfImportOptions | Opsi. |

### Nilai Pengembalian

Itu[`PdfImporter`](../) .

### Lihat juga

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* ruang nama [Aspose.Note.Importing](../../pdfimporter/)
* perakitan [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

Mengimpor konten dokumen PDF dari file tertentu.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| file | String | File PDF. |
| options | PdfImportOptions | Opsi. |

### Nilai Pengembalian

Itu[`PdfImporter`](../) .

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* ruang nama [Aspose.Note.Importing](../../pdfimporter/)
* perakitan [Aspose.Note](../../../)


