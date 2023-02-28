---
title: CheckBox.SetCompleted
second_title: Aspose.Note voor .NET API-referentie
description: CheckBox methode. Stelt de tag in op voltooide status.
type: docs
weight: 70
url: /nl/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

Stelt de tag in op voltooide status.

```csharp
public void SetCompleted(DateTime completedTime)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| completedTime | DateTime | De voltooide tijd. |

### Zie ook

* class [CheckBox](../)
* naamruimte [Aspose.Note](../../checkbox/)
* montage [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

Stelt de tag in op de voltooide status met de huidige tijd als voltooide tijd.

```csharp
public void SetCompleted()
```

### Voorbeelden

Laat zien hoe u alle selectievakje-items met betrekking tot 'Project C' kunt voltooien.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
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

### Zie ook

* class [CheckBox](../)
* naamruimte [Aspose.Note](../../checkbox/)
* montage [Aspose.Note](../../../)


