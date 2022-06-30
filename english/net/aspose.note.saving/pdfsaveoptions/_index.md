---
title: PdfSaveOptions
second_title: Aspose.Note for .NET API Reference
description: Allows to specify additional options when rendering document pages to PDF.
type: docs
weight: 820
url: /net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Allows to specify additional options when rendering document pages to PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Gets or sets font's settings to be used while saving |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression) { get; set; } | Gets or sets the type of compression applied to images in the PDF file. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality) { get; set; } | Gets or sets a value determining the quality of the JPEG images inside PDF document. The value may vary from 0 to 100 where 0 means worst quality but maximum compression and 100 means best quality but minimum compression. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Gets or sets the number of pages to save. By default is MaxValue which means all pages of the document will be rendered. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Gets or sets the index of the first page to save. By default is 0. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm) { get; set; } | Gets or sets algorithm used for page splitting. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Gets the format in which the document is saved. |

### Examples

Shows how to save notebook in pdf format with specified options.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Save the Notebook
notebook.Save(dataDir, notebookSaveOptions);
```

When long OneNote pages are saved in pdf format they are split across pages. The sample shows how to configure the splitting logic of objects located on page's breaks.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// or
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Shows how to save a document in pdf format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Set page index of first page to be saved
                              PageIndex = 0,

                              // Set page count
                              PageCount = 1,
                          };

// Save the document as PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Shows how to save a document in pdf format using specific settings.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Use Jpeg compression
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Quality for JPEG compression
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

When long OneNote pages are saved in pdf format they are split across pages. The example shows how to configure the splitting logic of objects located on page's breaks.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Or
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### See Also

* class [SaveOptions](../saveoptions)
* namespace [Aspose.Note.Saving](../../aspose.note.saving)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
