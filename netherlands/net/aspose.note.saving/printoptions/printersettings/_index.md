---
title: PrintOptions.PrinterSettings
second_title: Aspose.Note voor .NET API-referentie
description: PrintOptions eigendom. Haalt of stelt de printerinstellingen in.
type: docs
weight: 40
url: /nl/net/aspose.note.saving/printoptions/printersettings/
---
## PrintOptions.PrinterSettings property

Haalt of stelt de printerinstellingen in.

```csharp
public PrinterSettings PrinterSettings { get; set; }
```

### Voorbeelden

Laat zien hoe u een document naar een printer kunt sturen met behulp van het standaard Windows-dialoogvenster met gespecificeerde opties.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* class [PrintOptions](../)
* naamruimte [Aspose.Note.Saving](../../printoptions/)
* montage [Aspose.Note](../../../)


