---
title: INoteTag.Highlight
second_title: Aspose.Note for .NET API Reference
description: INoteTag property. Gets or sets the highlight color
type: docs
weight: 20
url: /net/aspose.note/inotetag/highlight/
---
## INoteTag.Highlight property

Gets or sets the highlight color.

```csharp
public Color Highlight { get; set; }
```

## Examples

Shows how to access details of a tag.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Get all RichText nodes
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterate through each node
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Retrieve properties
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### See Also

* interface [INoteTag](../)
* namespace [Aspose.Note](../../inotetag/)
* assembly [Aspose.Note](../../../)


