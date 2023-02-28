---
title: PrintOptions.PageSplittingAlgorithm
second_title: Aspose.Note för .NET API-referens
description: PrintOptions fast egendom. Hämtar eller ställer in algoritm som används för siddelning.
type: docs
weight: 30
url: /sv/net/aspose.note.saving/printoptions/pagesplittingalgorithm/
---
## PrintOptions.PageSplittingAlgorithm property

Hämtar eller ställer in algoritm som används för siddelning.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### Fastighetsvärde

Den`PageSplittingAlgorithm` .

### Exempel

Visar hur man skickar dokument till en skrivare med standard Windows-dialogruta med angivna alternativ.

```csharp
// Sökvägen till dokumentkatalogen.
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

### Se även

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PrintOptions](../)
* namnutrymme [Aspose.Note.Saving](../../printoptions/)
* hopsättning [Aspose.Note](../../../)


