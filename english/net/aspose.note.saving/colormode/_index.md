---
title: Enum ColorMode
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.ColorMode enum. The color mode of the image
type: docs
weight: 650
url: /net/aspose.note.saving/colormode/
---
## ColorMode enumeration

The color mode of the image.

```csharp
public enum ColorMode
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Normal | `0` | Full color image |
| GrayScale | `1` | Gray scale image |
| BlackAndWhite | `2` | Binary image: only black and white colors are used |

## Examples

Shows how to save a document as grayscale image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Save the document as gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

Shows how to save a document as image in Tiff format using CCITT Group 3 fax compression.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Save the document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

Shows how to save a document as binary image using Otsu's method.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Save the document as gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

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

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


