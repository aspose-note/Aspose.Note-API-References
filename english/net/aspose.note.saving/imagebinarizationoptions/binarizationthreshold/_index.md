---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note for .NET API Reference
description: ImageBinarizationOptions property. Gets or sets threshold value for fixed threshold binarization method. The default value is 128
type: docs
weight: 30
url: /net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

Gets or sets threshold value for fixed threshold binarization method. The default value is 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

## Examples

Shows how to save a document as binary image using fixed threshold.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Save the document as gif.
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

### See Also

* class [ImageBinarizationOptions](../)
* namespace [Aspose.Note.Saving](../../imagebinarizationoptions/)
* assembly [Aspose.Note](../../../)


