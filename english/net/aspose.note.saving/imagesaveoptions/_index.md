---
title: ImageSaveOptions
second_title: Aspose.Note for .NET API Reference
description: 
type: docs
weight: 670
url: /net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Allows to specify additional options when rendering document pages to images.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions)(SaveFormat) | Initializes a new instance of the [`ImageSaveOptions`](../imagesaveoptions) class. |

## Properties

| Name | Description |
| --- | --- |
| [BinarizationOptions](binarizationoptions) { get; set; } | Gets or sets options for image's binarization. |
| [ColorMode](colormode) { get; set; } | Gets or sets [`ColorMode`](./colormode) for the output image. |
| [Quality](quality) { get; set; } | Gets or sets a value determining the quality of saved image. This value is passed to codec as System.Drawing.Imaging.Encoder.Quality parameter. |
| [Resolution](resolution) { get; set; } | Gets or sets the resolution for the generated images, in dots per inch. |
| [TiffCompression](tiffcompression) { get; set; } | Gets or sets the type of compression to use when saving generated images to the TIFF format. |

### Examples

Shows how to save a document as image in Jpeg format using SaveFormat.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Save the document.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Shows how to set a image quality when saving document as image in JPEG format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Save the document.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Shows how to save a document as image in Bmp format using ImageSaveOptions.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Save the document.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Shows how to set a image resolution when saving document as image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Save the document.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

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

Shows how to save a document as image in Tiff format using PackBits compression.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Save the document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Shows how to save notebook as image with specified options.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Save the Notebook
notebook.Save(dataDir, notebookSaveOptions);
```

Shows how to save a document as image in Tiff format using Jpeg compression.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Save the document.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Shows how to save flattened notebook as image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Save the Notebook
notebook.Save(dataDir, notebookSaveOptions);
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

Shows how to save a document in png format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize ImageSaveOptions object 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Set page index
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Save the document as PNG.
oneFile.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions)
* namespace [Aspose.Note.Saving](../../aspose.note.saving)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
