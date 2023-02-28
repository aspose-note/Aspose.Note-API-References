---
title: Class ImageBinarizationOptions
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.ImageBinarizationOptions klas. Opties voor binarisatie van afbeeldingen.
type: docs
weight: 710
url: /nl/net/aspose.note.saving/imagebinarizationoptions/
---
## ImageBinarizationOptions class

Opties voor binarisatie van afbeeldingen.

```csharp
public class ImageBinarizationOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [ImageBinarizationOptions](imagebinarizationoptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BinarizationMethod](../../aspose.note.saving/imagebinarizationoptions/binarizationmethod/) { get; set; } | Haalt de binarisatiemethode op of stelt deze in. De standaardwaarde isFixedThreshold . |
| [BinarizationThreshold](../../aspose.note.saving/imagebinarizationoptions/binarizationthreshold/) { get; set; } | Haalt de drempelwaarde op of stelt deze in voor de binarisatiemethode met vaste drempel. De standaardwaarde is 128. |

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


