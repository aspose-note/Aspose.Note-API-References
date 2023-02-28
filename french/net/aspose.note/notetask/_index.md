---
title: Class NoteTask
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.NoteTask classe. Représente une tâche de note.
type: docs
weight: 400
url: /fr/net/aspose.note/notetask/
---
## NoteTask class

Représente une tâche de note.

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Obtient une valeur indiquant si le CheckBox est dans l'état coché. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Obtient ou définit l'heure de fin. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Obtient ou définit l'heure de création. |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | Obtient ou définit la date d'échéance. |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | Obtient ou définit l'icône. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Obtient le texte de l'étiquette. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Obtient ou définit le statut. |

## Méthodes

| Nom | La description |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | Crée une nouvelle tâche de note avec l'icône NoFollowUpDateFlag et la date d'échéance spécifiée. |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | Crée une nouvelle tâche de note avec l'icône FollowUpNextWeekFlag. |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | Crée une nouvelle tâche de note avec l'icône FollowUpThisWeekFlag. |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | Crée une nouvelle tâche de note avec l'icône FollowUpTodayFlag. |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | Crée une nouvelle tâche de note avec l'icône FollowUpTomorrowFlag. |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | Crée une nouvelle tâche de note avec l'icône NoFollowUpDateFlag. |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | Sert de fonction de hachage pour le type. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | Définit la balise à l'état terminé en utilisant l'heure actuelle comme heure terminée. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | Définit la balise à l'état terminé. |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | Définit la balise à l'état ouvert. |

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

Montre comment accéder aux détails des tâches Outlook.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Tasks();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Récupère tous les nœuds RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Itérer à travers chaque nœud
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Récupérer les propriétés
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Voir également

* class [CheckBox](../checkbox/)
* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


