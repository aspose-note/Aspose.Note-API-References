---
title: PrintOptions.PageSplittingAlgorithm
second_title: Référence de l'API Aspose.Note pour .NET
description: PrintOptions propriété. Obtient ou définit lalgorithme utilisé pour le fractionnement de page.
type: docs
weight: 30
url: /fr/net/aspose.note.saving/printoptions/pagesplittingalgorithm/
---
## PrintOptions.PageSplittingAlgorithm property

Obtient ou définit l'algorithme utilisé pour le fractionnement de page.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### Valeur de la propriété

Le`PageSplittingAlgorithm` .

### Exemples

Montre comment envoyer un document à une imprimante à l'aide de la boîte de dialogue Windows standard avec les options spécifiées.

```csharp
// Le chemin d'accès au répertoire des documents.
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

### Voir également

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PrintOptions](../)
* espace de noms [Aspose.Note.Saving](../../printoptions/)
* Assemblée [Aspose.Note](../../../)


