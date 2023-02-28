---
title: ImageBinarizationOptions.BinarizationMethod
second_title: Aspose.Note voor .NET API-referentie
description: ImageBinarizationOptions eigendom. Haalt de binarisatiemethode op of stelt deze in. De standaardwaarde isFixedThreshold .
type: docs
weight: 20
url: /nl/net/aspose.note.saving/imagebinarizationoptions/binarizationmethod/
---
## ImageBinarizationOptions.BinarizationMethod property

Haalt de binarisatiemethode op of stelt deze in. De standaardwaarde isFixedThreshold .

```csharp
public BinarizationMethod BinarizationMethod { get; set; }
```

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

* enum [BinarizationMethod](../../binarizationmethod/)
* class [ImageBinarizationOptions](../)
* naamruimte [Aspose.Note.Saving](../../imagebinarizationoptions/)
* montage [Aspose.Note](../../../)


