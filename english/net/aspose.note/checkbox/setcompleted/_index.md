---
title: CheckBox.SetCompleted
second_title: Aspose.Note for .NET API Reference
description: CheckBox method. Sets the tag to completed state
type: docs
weight: 70
url: /net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

Sets the tag to completed state.

```csharp
public void SetCompleted(DateTime completedTime)
```

| Parameter | Type | Description |
| --- | --- | --- |
| completedTime | DateTime | The completed time. |

### See Also

* class [CheckBox](../)
* namespace [Aspose.Note](../../checkbox/)
* assembly [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

Sets the tag to completed state using current time as completed time.

```csharp
public void SetCompleted()
```

## Examples

Shows how to make completed all checkbox items related to 'Project C'.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Load the document into Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

### See Also

* class [CheckBox](../)
* namespace [Aspose.Note](../../checkbox/)
* assembly [Aspose.Note](../../../)


