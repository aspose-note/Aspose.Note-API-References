---
title: PrintOptions.PrinterSettings
second_title: Aspose.Note für .NET-API-Referenz
description: PrintOptions eigendom. Ruft die Druckereinstellungen ab oder legt sie fest.
type: docs
weight: 40
url: /de/net/aspose.note.saving/printoptions/printersettings/
---
## PrintOptions.PrinterSettings property

Ruft die Druckereinstellungen ab oder legt sie fest.

```csharp
public PrinterSettings PrinterSettings { get; set; }
```

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

* class [PrintOptions](../)
* namensraum [Aspose.Note.Saving](../../printoptions/)
* Montage [Aspose.Note](../../../)


