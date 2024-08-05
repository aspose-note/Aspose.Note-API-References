---
title: Class KeepSolidObjectsAlgorithm
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.KeepSolidObjectsAlgorithm class. Shifts full object to the next page in case it doesnt fit in original page
type: docs
weight: 810
url: /net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

Shifts full object to the next page in case it doesn't fit in original page.

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## Constructors

| Name | Description |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | Initializes a new instance of the `KeepSolidObjectsAlgorithm` class using default height limit of cloned part. |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | Initializes a new instance of the `KeepSolidObjectsAlgorithm` class using specific height limit of cloned part. |

## Properties

| Name | Description |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | Gets the height limit of cloned part. |

## Fields

| Name | Description |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | The default max size of cloned part. |

## Examples

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

Shows how to sent document to a printer using standard Windows dialog with specified options.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
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

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


