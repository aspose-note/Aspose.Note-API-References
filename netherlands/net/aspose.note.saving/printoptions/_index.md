---
title: Class PrintOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.PrintOptions klas. Opties gebruikt om een document af te drukken.
type: docs
weight: 860
url: /nl/net/aspose.note.saving/printoptions/
---
## PrintOptions class

Opties gebruikt om een document af te drukken.

```csharp
public class PrintOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [PrintOptions](printoptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | Haalt de documentnaam op die moet worden weergegeven (bijvoorbeeld in een afdrukstatusdialoogvenster of printerwachtrij) tijdens het afdrukken van het document. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | Haalt of stelt het algoritme in dat wordt gebruikt voor het splitsen van pagina's. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | Haalt of stelt de printerinstellingen in. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | Hiermee wordt de resolutie voor de gegenereerde afbeeldingen opgehaald of ingesteld, in dots per inch. |

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

* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


