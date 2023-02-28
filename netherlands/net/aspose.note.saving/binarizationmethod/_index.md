---
title: Enum BinarizationMethod
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.BinarizationMethod opsomming. Specificeert de binarisatiemethode voor een afbeelding.
type: docs
weight: 560
url: /nl/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

Specificeert de binarisatiemethode voor een afbeelding.

```csharp
public enum BinarizationMethod
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| FixedThreshold | `0` | De binarisatie van de afbeelding wordt uitgevoerd met behulp van een opgegeven vaste drempel. |
| Otsu | `1` | De binarisatie van de afbeelding wordt adaptief uitgevoerd met behulp van de methode van Otsu om de drempel te evalueren. |

### Voorbeelden

Laat zien hoe u een document opslaat als binaire afbeelding met behulp van de methode van Otsu.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Sla het document op als gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Laat zien hoe u een document opslaat als binaire afbeelding met een vaste drempel.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Sla het document op als gif.
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

### Zie ook

* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


