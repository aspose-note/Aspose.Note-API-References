---
title: CheckBox.SetOpen
second_title: Aspose.Note voor .NET API-referentie
description: CheckBox methode. Stelt de tag in op open status.
type: docs
weight: 80
url: /nl/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

Stelt de tag in op open status.

```csharp
public virtual void SetOpen()
```

### Voorbeelden

Laat zien hoe u alle selectievakje-items met betrekking tot 'Project C' kunt openen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
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

### Zie ook

* class [CheckBox](../)
* naamruimte [Aspose.Note](../../checkbox/)
* montage [Aspose.Note](../../../)


