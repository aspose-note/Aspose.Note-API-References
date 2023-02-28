---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Référence de l'API Aspose.Note pour .NET
description: ImageBinarizationOptions propriété. Obtient ou définit la valeur de seuil pour la méthode de binarisation à seuil fixe. La valeur par défaut est 128.
type: docs
weight: 30
url: /fr/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

Obtient ou définit la valeur de seuil pour la méthode de binarisation à seuil fixe. La valeur par défaut est 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

### Exemples

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

* class [ImageBinarizationOptions](../)
* espace de noms [Aspose.Note.Saving](../../imagebinarizationoptions/)
* Assemblée [Aspose.Note](../../../)


