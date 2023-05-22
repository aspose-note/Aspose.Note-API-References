---
title: RichText.LastModifiedTime
second_title: Aspose.Note for .NET API Reference
description: RichText property. Gets or sets the last modified time
type: docs
weight: 30
url: /net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

Gets or sets the last modified time.

```csharp
public DateTime LastModifiedTime { get; set; }
```

## Examples

Let's emphasize latest text's changes by highlighting.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Get RichText nodes modified last week.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Set highlight color
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Set highlight color
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### See Also

* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)


