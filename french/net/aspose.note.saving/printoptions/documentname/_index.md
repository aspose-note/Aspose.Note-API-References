---
title: PrintOptions.DocumentName
second_title: Référence de l'API Aspose.Note pour .NET
description: PrintOptions propriété. Obtient ou définit le nom du document à afficher par exemple dans une boîte de dialogue détat dimpression ou une file dattente dimpression lors de limpression du document.
type: docs
weight: 20
url: /fr/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

Obtient ou définit le nom du document à afficher (par exemple, dans une boîte de dialogue d'état d'impression ou une file d'attente d'impression) lors de l'impression du document.

```csharp
public string DocumentName { get; set; }
```

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

* class [PrintOptions](../)
* espace de noms [Aspose.Note.Saving](../../printoptions/)
* Assemblée [Aspose.Note](../../../)


