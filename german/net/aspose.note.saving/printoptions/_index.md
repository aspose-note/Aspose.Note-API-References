---
title: Class PrintOptions
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Saving.PrintOptions klas. Optionen zum Drucken eines Dokuments.
type: docs
weight: 860
url: /de/net/aspose.note.saving/printoptions/
---
## PrintOptions class

Optionen zum Drucken eines Dokuments.

```csharp
public class PrintOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [PrintOptions](printoptions/)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | Ruft den Dokumentnamen ab oder legt ihn fest, der angezeigt werden soll (z. B. in einem Druckstatusdialogfeld oder einer Druckerwarteschlange), während das Dokument gedruckt wird. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | Ruft den für die Seitenaufteilung verwendeten Algorithmus ab oder legt ihn fest. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | Ruft die Druckereinstellungen ab oder legt sie fest. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | Ruft die Auflösung für die generierten Bilder in Punkten pro Zoll ab oder legt sie fest. |

### Beispiele

Zeigt, wie ein Dokument mithilfe des Windows-Standarddialogs mit festgelegten Optionen an einen Drucker gesendet wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

### Siehe auch

* namensraum [Aspose.Note.Saving](../../aspose.note.saving/)
* Montage [Aspose.Note](../../)


