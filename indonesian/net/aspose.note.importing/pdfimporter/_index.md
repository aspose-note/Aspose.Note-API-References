---
title: Class PdfImporter
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Importing.PdfImporter kelas. Kelas yang menyediakan api untuk mengimpor konten dari dokumen dalam format PDF. Api memungkinkan untuk mengimpor dari dokumen PDF yang terletak di file atau di aliran menggunakan opsi yang ditentukan. Opsi impor diteruskan menggunakanPdfImportOptions .
type: docs
weight: 270
url: /id/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

Kelas yang menyediakan api untuk mengimpor konten dari dokumen dalam format PDF. Api memungkinkan untuk mengimpor dari dokumen PDF yang terletak di file atau di aliran menggunakan opsi yang ditentukan. Opsi impor diteruskan menggunakan[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## Metode

| Nama | Keterangan |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | Mengimpor konten dokumen PDF dari aliran yang disediakan. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | Mengimpor konten dokumen PDF dari file tertentu. |

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

* ruang nama [Aspose.Note.Importing](../../aspose.note.importing/)
* perakitan [Aspose.Note](../../)


