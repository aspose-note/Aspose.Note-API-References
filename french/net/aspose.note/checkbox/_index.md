---
title: Class CheckBox
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.CheckBox classe. La classe de base pour les balises qui peuvent basculer leur état entre complet et incomplet.
type: docs
weight: 20
url: /fr/net/aspose.note/checkbox/
---
## CheckBox class

La classe de base pour les balises qui peuvent basculer leur état entre complet et incomplet.

```csharp
public abstract class CheckBox : ITag
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Obtient une valeur indiquant si le CheckBox est dans l'état coché. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Obtient ou définit l'heure de fin. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Obtient ou définit l'heure de création. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | Obtient ou définit l'icône. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Obtient le texte de l'étiquette. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Obtient ou définit le statut. |

## Méthodes

| Nom | La description |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | Définit la balise à l'état terminé en utilisant l'heure actuelle comme heure terminée. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | Définit la balise à l'état terminé. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | Définit la balise à l'état ouvert. |

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

* interface [ITag](../itag/)
* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


