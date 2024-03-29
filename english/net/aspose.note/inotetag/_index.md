---
title: Interface INoteTag
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.INoteTag interface. The interface for note tagsi.e. tags that are not associated with Outlook tasks
type: docs
weight: 180
url: /net/aspose.note/inotetag/
---
## INoteTag interface

The interface for note tags(i.e. tags that are not associated with Outlook tasks).

```csharp
public interface INoteTag : ITag
```

## Properties

| Name | Description |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | Gets or sets the font color. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | Gets or sets the highlight color. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | Gets or sets the label text. |

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

* interface [ITag](../itag/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


