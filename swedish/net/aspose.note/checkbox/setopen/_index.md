---
title: CheckBox.SetOpen
second_title: Aspose.Note för .NET API-referens
description: CheckBox metod. Ställer in taggen till öppet läge.
type: docs
weight: 80
url: /sv/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

Ställer in taggen till öppet läge.

```csharp
public virtual void SetOpen()
```

### Exempel

Visar hur man öppnar alla kryssrutor relaterade till 'Projekt C'.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tags();

// Ladda dokumentet i Aspose.Note.
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

### Se även

* class [CheckBox](../)
* namnutrymme [Aspose.Note](../../checkbox/)
* hopsättning [Aspose.Note](../../../)


