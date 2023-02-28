---
title: Class PrintOptions
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Saving.PrintOptions klass. Alternativ som används för att skriva ut ett dokument.
type: docs
weight: 860
url: /sv/net/aspose.note.saving/printoptions/
---
## PrintOptions class

Alternativ som används för att skriva ut ett dokument.

```csharp
public class PrintOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [PrintOptions](printoptions/)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | Hämtar eller ställer in dokumentnamnet som ska visas (till exempel i en utskriftsstatusdialogruta eller skrivarkö) under utskrift av dokumentet. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | Hämtar eller ställer in algoritm som används för siddelning. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | Hämtar eller ställer in skrivarinställningarna. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | Hämtar eller ställer in upplösningen för de genererade bilderna, i punkter per tum. |

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

* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving/)
* hopsättning [Aspose.Note](../../)


