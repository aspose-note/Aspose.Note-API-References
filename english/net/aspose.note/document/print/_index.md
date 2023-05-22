---
title: Document.Print
second_title: Aspose.Note for .NET API Reference
description: Document method. Prints the document using the default printer
type: docs
weight: 130
url: /net/aspose.note/document/print/
---
## Print() {#print}

Prints the document using the default printer.

```csharp
public void Print()
```

## Examples

Shows how to sent document to a printer using standard Windows dialog with default options.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
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

### See Also

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Print(PrintOptions) {#print_1}

Prints the document using the default printer.

```csharp
public void Print(PrintOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | PrintOptions | Options used to print a document. Can be null. |

### See Also

* class [PrintOptions](../../../aspose.note.saving/printoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


