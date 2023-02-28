---
title: Class CheckBox
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.CheckBox klas. De basisklasse voor tags die hun status kunnen schakelen tussen voltooid en onvolledig.
type: docs
weight: 20
url: /nl/net/aspose.note/checkbox/
---
## CheckBox class

De basisklasse voor tags die hun status kunnen schakelen tussen voltooid en onvolledig.

```csharp
public abstract class CheckBox : ITag
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Krijgt een waarde die aangeeft of de CheckBox in de gecontroleerde staat is. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Haalt of stelt de voltooide tijd in. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Haalt of stelt de aanmaaktijd in. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | Krijgt of stelt het pictogram in. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Haalt de labeltekst op. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Krijgt of stelt de status in. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | Stelt de tag in op de voltooide status met de huidige tijd als voltooide tijd. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | Stelt de tag in op voltooide status. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | Stelt de tag in op open status. |

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

### Zie ook

* interface [ITag](../itag/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


