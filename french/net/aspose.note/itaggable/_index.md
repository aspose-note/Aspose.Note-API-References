---
title: Interface ITaggable
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.ITaggable interface. Linterface pour les nœuds qui peuvent être marqués par des balises.
type: docs
weight: 240
url: /fr/net/aspose.note/itaggable/
---
## ITaggable interface

L'interface pour les nœuds qui peuvent être marqués par des balises.

```csharp
public interface ITaggable : INode
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Tags](../../aspose.note/itaggable/tags/) { get; } | Obtient la liste de toutes les balises. |

### Exemples

Montre comment générer un pdf contenant toutes les pages liées au 'Projet A'.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tags();

// Charge le document dans Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.Any(x => x.Label.Contains("Project A"))))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "ProjectA_Report.pdf"));
```

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

Montre comment ouvrir tous les éléments de case à cocher liés au "Projet C".

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tags();

// Charge le document dans Aspose.Note.
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

Montre comment générer un pdf contenant des pages avec des éléments marqués par des cases à cocher incomplètes et créés au cours de la semaine dernière.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tags();

// Charge le document dans Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<CheckBox>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteLastWeekReport.pdf"));
```

Montre comment générer un pdf contenant des pages avec des tâches Outlook incomplètes à terminer cette semaine.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tags();

// Charge le document dans Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "TagFile.one"));

var report = new Document();
var endOfWeek = DateTime.Today.AddDays(5 - (int)DateTime.Today.DayOfWeek);
foreach (var page in oneFile)
{
    if (page.GetChildNodes<ITaggable>().Any(e => e.Tags.OfType<NoteTask>().Any(x => !x.Checked && DateTime.UtcNow.Subtract(TimeSpan.FromDays(7)) <= x.CreationTime && x.DueDate <= endOfWeek)))
    {
        report.AppendChildLast(page.Clone());
    }
}

report.Save(Path.Combine(dataDir, "IncompleteTasksForThisWeekReport.pdf"));
```

### Voir également

* interface [INode](../inode/)
* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


