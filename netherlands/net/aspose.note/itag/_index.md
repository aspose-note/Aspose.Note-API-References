---
title: Interface ITag
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.ITag koppel. De interface voor alle soorten tags.
type: docs
weight: 230
url: /nl/net/aspose.note/itag/
---
## ITag interface

De interface voor alle soorten tags.

```csharp
public interface ITag
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CompletedTime](../../aspose.note/itag/completedtime/) { get; } | Haalt of stelt de voltooide tijd in. |
| [CreationTime](../../aspose.note/itag/creationtime/) { get; set; } | Haalt of stelt de aanmaaktijd in. |
| [Icon](../../aspose.note/itag/icon/) { get; } | Krijgt of stelt het pictogram in. |
| [Label](../../aspose.note/itag/label/) { get; } | Haalt de labeltekst op. |
| [Status](../../aspose.note/itag/status/) { get; } | Krijgt of stelt de status in. |

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

Laat zien hoe u een pdf kunt genereren met pagina's met items die zijn gemarkeerd met onvolledige selectievakjes en die in de afgelopen week zijn gemaakt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
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

Laat zien hoe u een pdf kunt genereren met pagina's met onvoltooide Outlook-taken die deze week moeten worden voltooid.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
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

Laat zien hoe u toegang krijgt tot de details van een tag.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Haal alle RichText-knooppunten op
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Doorloop elk knooppunt
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Eigenschappen ophalen
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### Zie ook

* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


