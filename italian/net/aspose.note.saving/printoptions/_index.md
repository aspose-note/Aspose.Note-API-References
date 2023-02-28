---
title: Class PrintOptions
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Saving.PrintOptions classe. Opzioni utilizzate per stampare un documento.
type: docs
weight: 860
url: /it/net/aspose.note.saving/printoptions/
---
## PrintOptions class

Opzioni utilizzate per stampare un documento.

```csharp
public class PrintOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PrintOptions](printoptions/)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | Ottiene o imposta il nome del documento da visualizzare (ad esempio, in una finestra di dialogo sullo stato della stampa o in una coda di stampa) durante la stampa del documento. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | Ottiene o imposta l'algoritmo utilizzato per la suddivisione della pagina. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | Ottiene o imposta le impostazioni della stampante. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | Ottiene o imposta la risoluzione per le immagini generate, in punti per pollice. |

### Esempi

Mostra come inviare un documento a una stampante utilizzando la finestra di dialogo standard di Windows con le opzioni specificate.

```csharp
// Il percorso della directory dei documenti.
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

### Guarda anche

* spazio dei nomi [Aspose.Note.Saving](../../aspose.note.saving/)
* assemblea [Aspose.Note](../../)


