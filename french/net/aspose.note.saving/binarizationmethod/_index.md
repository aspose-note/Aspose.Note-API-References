---
title: Enum BinarizationMethod
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Saving.BinarizationMethod énumération. Spécifie la méthode de binarisation pour une image.
type: docs
weight: 560
url: /fr/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

Spécifie la méthode de binarisation pour une image.

```csharp
public enum BinarizationMethod
```

### Valeurs

| Nom | Évaluer | La description |
| --- | --- | --- |
| FixedThreshold | `0` | La binarisation de l'image est effectuée à l'aide d'un seuil fixe spécifié. |
| Otsu | `1` | La binarisation de l'image est effectuée de manière adaptative à l'aide de la méthode d'Otsu pour évaluer le seuil. |

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


