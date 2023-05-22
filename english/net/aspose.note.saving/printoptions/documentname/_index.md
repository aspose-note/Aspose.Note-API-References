---
title: PrintOptions.DocumentName
second_title: Aspose.Note for .NET API Reference
description: PrintOptions property. Gets or sets the document name to display for example in a print status dialog box or printer queue while printing the document
type: docs
weight: 20
url: /net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

Gets or sets the document name to display (for example, in a print status dialog box or printer queue) while printing the document.

```csharp
public string DocumentName { get; set; }
```

## Examples

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

### See Also

* class [PrintOptions](../)
* namespace [Aspose.Note.Saving](../../printoptions/)
* assembly [Aspose.Note](../../../)


