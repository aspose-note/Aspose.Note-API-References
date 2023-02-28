---
title: Class PrintOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Saving.PrintOptions classe. Options utilisées pour imprimer un document.
type: docs
weight: 860
url: /fr/net/aspose.note.saving/printoptions/
---
## PrintOptions class

Options utilisées pour imprimer un document.

```csharp
public class PrintOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [PrintOptions](printoptions/)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | Obtient ou définit le nom du document à afficher (par exemple, dans une boîte de dialogue d'état d'impression ou une file d'attente d'impression) lors de l'impression du document. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | Obtient ou définit l'algorithme utilisé pour le fractionnement de page. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | Obtient ou définit les paramètres de l'imprimante. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | Obtient ou définit la résolution des images générées, en points par pouce. |

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

* espace de noms [Aspose.Note.Saving](../../aspose.note.saving/)
* Assemblée [Aspose.Note](../../)


