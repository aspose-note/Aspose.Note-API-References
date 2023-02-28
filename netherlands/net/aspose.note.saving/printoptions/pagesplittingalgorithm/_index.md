---
title: PrintOptions.PageSplittingAlgorithm
second_title: Aspose.Note voor .NET API-referentie
description: PrintOptions eigendom. Haalt of stelt het algoritme in dat wordt gebruikt voor het splitsen van paginas.
type: docs
weight: 30
url: /nl/net/aspose.note.saving/printoptions/pagesplittingalgorithm/
---
## PrintOptions.PageSplittingAlgorithm property

Haalt of stelt het algoritme in dat wordt gebruikt voor het splitsen van pagina's.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### Eigendoms-waarde

De`PageSplittingAlgorithm` .

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

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PrintOptions](../)
* naamruimte [Aspose.Note.Saving](../../printoptions/)
* montage [Aspose.Note](../../../)


