---
title: Image.OriginalWidth
second_title: Aspose.Note for .NET API Reference
description: Image property. Gets the original width. This is the original width of the image before resizing
type: docs
weight: 150
url: /net/aspose.note/image/originalwidth/
---
## Image.OriginalWidth property

Gets the original width. This is the original width of the image, before resizing.

```csharp
public float OriginalWidth { get; }
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

### See Also

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


