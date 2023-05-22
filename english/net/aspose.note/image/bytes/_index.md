---
title: Image.Bytes
second_title: Aspose.Note for .NET API Reference
description: Image property. Gets the image data store
type: docs
weight: 50
url: /net/aspose.note/image/bytes/
---
## Image.Bytes property

Gets the image data store.

```csharp
public byte[] Bytes { get; }
```

## Examples

Shows how to get an image from a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Get all Image nodes
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Save image bytes to a file
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### See Also

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


