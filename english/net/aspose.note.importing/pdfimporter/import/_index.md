---
title: PdfImporter.Import
second_title: Aspose.Note for .NET API Reference
description: PdfImporter method. Imports content of PDF document from a provided stream
type: docs
weight: 10
url: /net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

Imports content of PDF document from a provided stream.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| options | PdfImportOptions | The options. |

### Return Value

The [`PdfImporter`](../).

### See Also

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* namespace [Aspose.Note.Importing](../../pdfimporter/)
* assembly [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

Imports content of PDF document from a specified file.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| file | String | The PDF file. |
| options | PdfImportOptions | The options. |

### Return Value

The [`PdfImporter`](../).

## Examples

Shows how to import all pages from PDF document grouping every 5 pages to a single OneNote page.

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

### See Also

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* namespace [Aspose.Note.Importing](../../pdfimporter/)
* assembly [Aspose.Note](../../../)


