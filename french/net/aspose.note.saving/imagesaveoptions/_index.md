---
title: Class ImageSaveOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Saving.ImageSaveOptions classe. Permet de spécifier des options supplémentaires lors du rendu des pages de document en images.
type: docs
weight: 720
url: /fr/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Permet de spécifier des options supplémentaires lors du rendu des pages de document en images.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | Initialise une nouvelle instance du`ImageSaveOptions` classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | Obtient ou définit les options de binarisation de l'image. |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | Obtient ou définit[`ColorMode`](./colormode/) pour l'image de sortie. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Obtient ou définit les paramètres de police à utiliser lors de l'enregistrement |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Obtient ou définit le nombre de pages à enregistrer. Par défaut estMaxValue ce qui signifie que toutes les pages du document seront rendues. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Obtient ou définit l'index de la première page à enregistrer. Par défaut est 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | Obtient ou définit une valeur déterminant la qualité de l'image enregistrée. Cette valeur est transmise au codec en tant que paramètre System.Drawing.Imaging.Encoder.Quality. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | Obtient ou définit la résolution des images générées, en points par pouce. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Obtient le format dans lequel le document est enregistré. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | Obtient ou définit le type de compression à utiliser lors de l'enregistrement des images générées au format TIFF. |

### Exemples

Montre comment enregistrer un document en tant qu'image au format Jpeg à l'aide de SaveFormat.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Enregistre le document.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Montre comment définir une qualité d'image lors de l'enregistrement d'un document en tant qu'image au format JPEG.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Enregistre le document.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Montre comment enregistrer un document en tant qu'image au format Bmp à l'aide d'ImageSaveOptions.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Enregistre le document.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Montre comment définir une résolution d'image lors de l'enregistrement d'un document en tant qu'image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Enregistre le document.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Montre comment enregistrer un document en tant qu'image en niveaux de gris.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Enregistrez le document au format gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Montre comment enregistrer un document en tant qu'image au format Tiff à l'aide de la compression PackBits.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Enregistre le document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Montre comment enregistrer le bloc-notes en tant qu'image avec les options spécifiées.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Enregistrer le bloc-notes
notebook.Save(dataDir, notebookSaveOptions);
```

Montre comment enregistrer un document en tant qu'image au format Tiff à l'aide de la compression Jpeg.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Enregistre le document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Montre comment enregistrer un cahier aplati en tant qu'image.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Charger un bloc-notes OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Enregistrer le bloc-notes
notebook.Save(dataDir, notebookSaveOptions);
```

Montre comment enregistrer un document en tant qu'image au format Tiff à l'aide de la compression de télécopie CCITT Groupe 3.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Enregistre le document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

Montre comment enregistrer un document au format png.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialise l'objet ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Définir l'index de la page
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Enregistrez le document au format PNG.
oneFile.Save(dataDir, opts);
```

Montre comment enregistrer un document en tant qu'image binaire à l'aide de la méthode d'Otsu.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Enregistrez le document au format gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Montre comment enregistrer un document en tant qu'image binaire à l'aide d'un seuil fixe.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Enregistrez le document au format gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### Voir également

* class [SaveOptions](../saveoptions/)
* espace de noms [Aspose.Note.Saving](../../aspose.note.saving/)
* Assemblée [Aspose.Note](../../)


