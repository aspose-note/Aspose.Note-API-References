---
title: Page.GetChildNodes
second_title: Aspose.Note for .NET API Reference
description: Page method. Get all child nodes of the page by the node type
type: docs
weight: 150
url: /net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

Get all child nodes of the page by the node type.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parameter | Description |
| --- | --- |
| T1 | The type of elements in the returned list. |

### Return Value

A list of child nodes.

## Examples

Shows how to get all text from the document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Retrieve text
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Print text on the output screen
Console.WriteLine(text);
```

Shows how to get all text from the page.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Get list of page nodes
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Retrieve text
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Print text on the output screen
    Console.WriteLine(text);
}
```

Shows how to pass through all pages and make a replacement in the text.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Get all RichText nodes
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Replace text of a shape
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Save to any supported file format
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Shows how to pass through page's text and make a replacement.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Get all RichText nodes
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Replace text of a shape
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Save to any supported file format
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### See Also

* interface [INode](../../inode/)
* class [Page](../)
* namespace [Aspose.Note](../../page/)
* assembly [Aspose.Note](../../../)


