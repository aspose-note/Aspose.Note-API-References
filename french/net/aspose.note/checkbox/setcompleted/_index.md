---
title: CheckBox.SetCompleted
second_title: Référence de l'API Aspose.Note pour .NET
description: CheckBox méthode. Définit la balise à létat terminé.
type: docs
weight: 70
url: /fr/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

Définit la balise à l'état terminé.

```csharp
public void SetCompleted(DateTime completedTime)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| completedTime | DateTime | Le temps terminé. |

### Voir également

* class [CheckBox](../)
* espace de noms [Aspose.Note](../../checkbox/)
* Assemblée [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

Définit la balise à l'état terminé en utilisant l'heure actuelle comme heure terminée.

```csharp
public void SetCompleted()
```

### Exemples

Montre comment compléter tous les éléments de case à cocher liés au "Projet C".

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tags();

// Charge le document dans Aspose.Note.
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

### Voir également

* class [CheckBox](../)
* espace de noms [Aspose.Note](../../checkbox/)
* Assemblée [Aspose.Note](../../../)


