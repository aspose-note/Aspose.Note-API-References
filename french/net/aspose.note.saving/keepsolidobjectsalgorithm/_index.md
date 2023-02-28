---
title: Class KeepSolidObjectsAlgorithm
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Saving.KeepSolidObjectsAlgorithm classe. Déplace lobjet complet vers la page suivante au cas où il ne rentre pas dans la page dorigine.
type: docs
weight: 740
url: /fr/net/aspose.note.saving/keepsolidobjectsalgorithm/
---
## KeepSolidObjectsAlgorithm class

Déplace l'objet complet vers la page suivante au cas où il ne rentre pas dans la page d'origine.

```csharp
public class KeepSolidObjectsAlgorithm : PageSplittingAlgorithm
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor)() | Initialise une nouvelle instance du`KeepSolidObjectsAlgorithm` classe utilisant la limite de hauteur par défaut de la partie clonée. |
| [KeepSolidObjectsAlgorithm](keepsolidobjectsalgorithm/#constructor_1)(float) | Initialise une nouvelle instance du`KeepSolidObjectsAlgorithm` classe utilisant la limite de hauteur spécifique de la partie clonée. |

## Propriétés

| Nom | La description |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/heightlimitofclonedpart/) { get; } | Obtient la limite de hauteur de la pièce clonée. |

## Des champs

| Nom | La description |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keepsolidobjectsalgorithm/defaultheightlimitofclonedpart/) | La taille maximale par défaut de la pièce clonée. |

### Exemples

Montre comment enregistrer un bloc-notes au format pdf avec les options spécifiées.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Enregistrer le bloc-notes
notebook.Save(dataDir, notebookSaveOptions);
```

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

Lorsque de longues pages OneNote sont enregistrées au format pdf, elles sont réparties sur plusieurs pages. L'exemple montre comment configurer la logique de découpage des objets situés sur les sauts de page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Voir également

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* espace de noms [Aspose.Note.Saving](../../aspose.note.saving/)
* Assemblée [Aspose.Note](../../)


