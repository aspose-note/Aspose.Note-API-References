---
title: ImageBinarizationOptions.BinarizationMethod
second_title: Aspose.Note för .NET API-referens
description: ImageBinarizationOptions fast egendom. Hämtar eller ställer in binariseringsmetoden. Standardvärdet ärFixedThreshold .
type: docs
weight: 20
url: /sv/net/aspose.note.saving/imagebinarizationoptions/binarizationmethod/
---
## ImageBinarizationOptions.BinarizationMethod property

Hämtar eller ställer in binariseringsmetoden. Standardvärdet ärFixedThreshold .

```csharp
public BinarizationMethod BinarizationMethod { get; set; }
```

### Exempel

Visar hur man sparar ett dokument som binär bild med Otsus metod.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Spara dokumentet som gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Visar hur man sparar ett dokument som binär bild med hjälp av fast tröskel.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Spara dokumentet som gif.
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

### Se även

* enum [BinarizationMethod](../../binarizationmethod/)
* class [ImageBinarizationOptions](../)
* namnutrymme [Aspose.Note.Saving](../../imagebinarizationoptions/)
* hopsättning [Aspose.Note](../../../)


