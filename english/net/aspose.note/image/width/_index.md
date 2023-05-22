---
title: Image.Width
second_title: Aspose.Note for .NET API Reference
description: Image property. Gets or sets the width. This is the real width of the image in the MS OneNote document
type: docs
weight: 180
url: /net/aspose.note/image/width/
---
## Image.Width property

Gets or sets the width. This is the real width of the image in the MS OneNote document.

```csharp
public float Width { get; set; }
```

## Examples

Shows how to get image's meta information.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Get all Image nodes
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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


