---
title: Notebook.DisplayName
second_title: Aspose.Note for .NET API Reference
description: Notebook property. Gets or sets the display name
type: docs
weight: 40
url: /net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

Gets or sets the display name.

```csharp
public string DisplayName { get; set; }
```

## Examples

Shows how to remove a section from a notebook.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Load a OneNote Notebook
var notebook = new Notebook(dataDir + "test.onetoc2");

// Traverse through its child nodes for searching the desired child item
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Remove the Child Item from the Notebook
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Save the Notebook
notebook.Save(dataDir);
```

### See Also

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)


