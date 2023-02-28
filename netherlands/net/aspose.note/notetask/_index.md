---
title: Class NoteTask
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.NoteTask klas. Vertegenwoordigt een notitietaak.
type: docs
weight: 400
url: /nl/net/aspose.note/notetask/
---
## NoteTask class

Vertegenwoordigt een notitietaak.

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Krijgt een waarde die aangeeft of de CheckBox in de gecontroleerde staat is. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Haalt of stelt de voltooide tijd in. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Haalt of stelt de aanmaaktijd in. |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | Haalt of stelt de vervaldatum in. |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | Krijgt of stelt het pictogram in. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Haalt de labeltekst op. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Krijgt of stelt de status in. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | Maakt een nieuwe notitietaak met het NoFollowUpDateFlag-pictogram en de gespecificeerde vervaldatum. |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | Maakt een nieuwe notitietaak aan met het pictogram FollowUpNextWeekFlag. |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | Maakt een nieuwe notitietaak aan met het pictogram FollowUpThisWeekFlag. |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | Maakt een nieuwe notitietaak aan met het pictogram FollowUpTodayFlag. |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | Maakt een nieuwe notitietaak aan met het pictogram FollowUpTomorrowFlag. |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | Maakt een nieuwe notitietaak aan met het pictogram NoFollowUpDateFlag. |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | Dient als hash-functie voor het type. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | Stelt de tag in op de voltooide status met de huidige tijd als voltooide tijd. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | Stelt de tag in op voltooide status. |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | Stelt de tag in op open status. |

### Voorbeelden

Laat zien hoe je een pdf genereert met alle pagina's gerelateerd aan 'Project A'.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
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

Laat zien hoe u toegang krijgt tot de details van de taken van Outlook.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tasks();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle RichText-knooppunten op
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Doorloop elk knooppunt
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Eigenschappen ophalen
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Zie ook

* class [CheckBox](../checkbox/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


