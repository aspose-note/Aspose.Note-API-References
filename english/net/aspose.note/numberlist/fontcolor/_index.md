---
title: NumberList.FontColor
second_title: Aspose.Note for .NET API Reference
description: NumberList property. Gets or sets the font color
type: docs
weight: 30
url: /net/aspose.note/numberlist/fontcolor/
---
## NumberList.FontColor property

Gets or sets the font color.

```csharp
public Color FontColor { get; set; }
```

## Examples

Shows how to retrieve information about list's formatting.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Retrieve a collection nodes of the outline element
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Iterate through each node
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Retrieve font name
        Console.WriteLine("Font Name: " + list.Font);

        // Retrieve font length
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Retrieve font size
        Console.WriteLine("Font Size: " + list.FontSize);

        // Retrieve font color
        Console.WriteLine("Font Color: " + list.FontColor);

        // Retrieve format
        Console.WriteLine("Font format: " + list.Format);

        // Check bold
        Console.WriteLine("Is bold: " + list.IsBold);

        // Check italic
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### See Also

* class [NumberList](../)
* namespace [Aspose.Note](../../numberlist/)
* assembly [Aspose.Note](../../../)


