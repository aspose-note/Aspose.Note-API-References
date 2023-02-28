---
title: Class ImageBinarizationOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Saving.ImageBinarizationOptions classe. Options de binarisation de limage.
type: docs
weight: 710
url: /fr/net/aspose.note.saving/imagebinarizationoptions/
---
## ImageBinarizationOptions class

Options de binarisation de l'image.

```csharp
public class ImageBinarizationOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [ImageBinarizationOptions](imagebinarizationoptions/)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [BinarizationMethod](../../aspose.note.saving/imagebinarizationoptions/binarizationmethod/) { get; set; } | Obtient ou définit la méthode de binarisation. La valeur par défaut estFixedThreshold . |
| [BinarizationThreshold](../../aspose.note.saving/imagebinarizationoptions/binarizationthreshold/) { get; set; } | Obtient ou définit la valeur de seuil pour la méthode de binarisation à seuil fixe. La valeur par défaut est 128. |

### Exemples

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

* espace de noms [Aspose.Note.Saving](../../aspose.note.saving/)
* Assemblée [Aspose.Note](../../)


