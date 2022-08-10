---
title: PdfSaveOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Permet de spécifier des options supplémentaires lors du rendu des pages de document au format PDF.
type: docs
weight: 820
url: /fr/net/aspose.note.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Permet de spécifier des options supplémentaires lors du rendu des pages de document au format PDF.

```csharp
public sealed class PdfSaveOptions : SaveOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | Obtient ou définit les paramètres de police à utiliser lors de l'enregistrement |
| [ImageCompression](../../aspose.note.saving/pdfsaveoptions/imagecompression) { get; set; } | Obtient ou définit le type de compression appliqué aux images dans le fichier PDF. |
| [JpegQuality](../../aspose.note.saving/pdfsaveoptions/jpegquality) { get; set; } | Obtient ou définit une valeur déterminant la qualité des images JPEG dans le document PDF. La valeur peut varier de 0 à 100, où 0 signifie la pire qualité mais une compression maximale et 100 signifie la meilleure qualité mais une compression minimale. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | Obtient ou définit le nombre de pages à enregistrer. Par défaut estMaxValue ce qui signifie que toutes les pages du document seront rendues. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | Obtient ou définit l'index de la première page à enregistrer. Par défaut est 0. |
| [PageSplittingAlgorithm](../../aspose.note.saving/pdfsaveoptions/pagesplittingalgorithm) { get; set; } | Obtient ou définit l'algorithme utilisé pour le fractionnement de page. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | Obtient le format dans lequel le document est enregistré. |

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

Lorsque de longues pages OneNote sont enregistrées au format pdf, elles sont réparties sur plusieurs pages. L'exemple montre comment configurer la logique de fractionnement des objets situés sur les sauts de page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// ou
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Montre comment enregistrer un document au format pdf.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialise l'objet PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Définit l'index de la première page à enregistrer
                              PageIndex = 0,

                              // Définir le nombre de pages
                              PageCount = 1,
                          };

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Montre comment enregistrer un document au format pdf en utilisant des paramètres spécifiques.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialise l'objet PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Utiliser la compression Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualité pour la compression JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions)
* espace de noms [Aspose.Note.Saving](../../aspose.note.saving)
* Assemblée [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
