---
title: PrintOptions.Resolution
second_title: Aspose.Note per .NET API Reference
description: PrintOptions proprietà. Ottiene o imposta la risoluzione per le immagini generate in punti per pollice.
type: docs
weight: 50
url: /it/net/aspose.note.saving/printoptions/resolution/
---
## PrintOptions.Resolution property

Ottiene o imposta la risoluzione per le immagini generate, in punti per pollice.

```csharp
public float Resolution { get; set; }
```

### Osservazioni

Il valore predefinito è 96.

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

* class [PrintOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../printoptions/)
* assemblea [Aspose.Note](../../../)


