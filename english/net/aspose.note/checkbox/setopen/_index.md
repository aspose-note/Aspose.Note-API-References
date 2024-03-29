---
title: CheckBox.SetOpen
second_title: Aspose.Note for .NET API Reference
description: CheckBox method. Sets the tag to open state
type: docs
weight: 80
url: /net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

Sets the tag to open state.

```csharp
public virtual void SetOpen()
```

## Examples

Shows how to make open all checkbox items related to 'Project C'.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Load the document into Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

### See Also

* class [CheckBox](../)
* namespace [Aspose.Note](../../checkbox/)
* assembly [Aspose.Note](../../../)


