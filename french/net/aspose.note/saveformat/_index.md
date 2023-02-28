---
title: Enum SaveFormat
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.SaveFormat énumération. Indique le format dans lequel le document est enregistré.
type: docs
weight: 540
url: /fr/net/aspose.note/saveformat/
---
## SaveFormat enumeration

Indique le format dans lequel le document est enregistré.

```csharp
public enum SaveFormat
```

### Valeurs

| Nom | Évaluer | La description |
| --- | --- | --- |
| Png | `1` | Spécifie que la sortie est un fichier PNG. |
| Bmp | `2` | Spécifie que la sortie est un fichier BMP. |
| Jpeg | `3` | Spécifie que la sortie est un fichier JPEG. |
| Gif | `4` | Spécifie que la sortie est un fichier GIF. |
| Tiff | `5` | Spécifie que la sortie est un fichier TIFF. |
| Pdf | `6` | Spécifie que la sortie est un fichier PDF. |
| One | `7` | Spécifie que la sortie est un fichier OneNote. |
| Html | `8` | Spécifie que la sortie est un fichier HTML. |

### Exemples

Montre comment enregistrer un document à l'aide de l'énumération SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Montre comment enregistrer un document au format pdf en utilisant les paramètres par défaut.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Enregistrer le document au format PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

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

Montre comment enregistrer un document au format gif.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Enregistrez le document au format gif.
oneFile.Save(dataDir, SaveFormat.Gif);
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

* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


