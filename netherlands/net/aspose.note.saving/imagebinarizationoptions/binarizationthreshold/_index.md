---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note voor .NET API-referentie
description: ImageBinarizationOptions eigendom. Haalt de drempelwaarde op of stelt deze in voor de binarisatiemethode met vaste drempel. De standaardwaarde is 128.
type: docs
weight: 30
url: /nl/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

Haalt de drempelwaarde op of stelt deze in voor de binarisatiemethode met vaste drempel. De standaardwaarde is 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

### Voorbeelden

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

* class [ImageBinarizationOptions](../)
* naamruimte [Aspose.Note.Saving](../../imagebinarizationoptions/)
* montage [Aspose.Note](../../../)


