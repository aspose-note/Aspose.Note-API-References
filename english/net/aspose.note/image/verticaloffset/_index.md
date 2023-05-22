---
title: Image.VerticalOffset
second_title: Aspose.Note for .NET API Reference
description: Image property. Gets or sets the vertical offset
type: docs
weight: 170
url: /net/aspose.note/image/verticaloffset/
---
## Image.VerticalOffset property

Gets or sets the vertical offset.

```csharp
public float VerticalOffset { get; set; }
```

## Examples

Shows how to add an image from file to a document with user defined properties.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Load document from the stream.
Document doc = new Document(dataDir + "Aspose.one");

// Get the first page of the document.
Aspose.Note.Page page = doc.FirstChild;

// Load an image from the file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Change the image's size according to your needs (optional).
                              Width = 100,
                              Height = 100,

                              // Set the image's location in the page (optional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Set image alignment
                              Alignment = HorizontalAlignment.Right
                          };

// Add the image to the page.
page.AppendChildLast(image);
```

### See Also

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


