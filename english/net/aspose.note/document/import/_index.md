---
title: Document.Import
second_title: Aspose.Note for .NET API Reference
description: Document method. Imports a set of pages from provided PDF document
type: docs
weight: 110
url: /net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import_1}

Imports a set of pages from provided PDF document.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | A stream with PDF document. |
| importOptions | PdfImportOptions | Specifies the options how to import pages from PDF document. |
| mergeOptions | MergeOptions | Specifies the options how to merge provided pages. |

### Return Value

Returns the reference to the document.

### See Also

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_3}

Imports a set of pages from provided PDF document.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| file | String | A file with PDF document. |
| importOptions | PdfImportOptions | Specifies the options how to import pages from PDF document. |
| mergeOptions | MergeOptions | Specifies the options how to merge provided pages. |

### Return Value

Returns the reference to the document.

## Examples

Shows how to import all pages from a set of PDF documents page by page.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
```

Shows how to import a PDF file into a OneNote document.

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Pdf();

// Specify paths
var pdfFilePath = Path.Combine(dataDir, "sample.pdf");
var oneFilePath = Path.Combine(dataDir, "output.one");

// Import PDF into OneNote
var document = new Document();
document.Import(pdfFilePath);
document.Save(oneFilePath);
```

Shows how to import all pages from a set of PDF documents while inserting pages from every PDF document as children of a top level OneNote page.

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

Shows how to import all content from a set of PDF documents while merging pages from every PDF document to a single OneNote page.

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

### See Also

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Import(Stream, HtmlImportOptions, MergeOptions) {#import}

Imports a set of pages from provided HTML document.

```csharp
public Document Import(Stream stream, HtmlImportOptions importOptions, 
    MergeOptions mergeOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | A stream with HTML document. |
| importOptions | HtmlImportOptions | Specifies the options how to import pages from HTML document. |
| mergeOptions | MergeOptions | Specifies the options how to merge provided pages. |

### Return Value

Returns the reference to the document.

### See Also

* class [HtmlImportOptions](../../../aspose.note.importing/htmlimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Import(string, HtmlImportOptions, MergeOptions) {#import_2}

Imports a set of pages from provided HTML document.

```csharp
public Document Import(string file, HtmlImportOptions importOptions, 
    MergeOptions mergeOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| file | String | A file with HTML document. |
| importOptions | HtmlImportOptions | Specifies the options how to import pages from HTML document. |
| mergeOptions | MergeOptions | Specifies the options how to merge provided pages. |

### Return Value

Returns the reference to the document.

## Examples

Shows how to import an HTML file into a OneNote document.

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Html();

var htmlFilePath = Path.Combine(dataDir, "sample.html");
var oneFilePath = Path.Combine(dataDir, "output.one");

// Import HTML into OneNote
var doc = new Document();
doc.Import(htmlFilePath, new HtmlImportOptions());
doc.Save(oneFilePath);
```

Shows how to import a Markdown file into a OneNote document.

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Markdown();

var mdFilePath = Path.Combine(dataDir, "sample.md");
var htmlFilePath = Path.Combine(dataDir, "temp.html");
var oneFilePath = Path.Combine(dataDir, "output.one");

// Convert Markdown to HTML
Converter.ConvertMarkdown(mdFilePath, htmlFilePath);

// Import HTML into OneNote
var document = new Document();
document.Import(htmlFilePath, new HtmlImportOptions());
document.Save(oneFilePath);

Console.WriteLine("\nMarkdown document imported into OneNote successfully.");
```

### See Also

* class [HtmlImportOptions](../../../aspose.note.importing/htmlimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


