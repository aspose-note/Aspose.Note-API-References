---
title: CheckBox.Checked
second_title: Aspose.Note für .NET-API-Referenz
description: CheckBox eigendom. Ruft einen Wert ab der angibt ob sich die CheckBox im aktivierten Zustand befindet.
type: docs
weight: 10
url: /de/net/aspose.note/checkbox/checked/
---
## CheckBox.Checked property

Ruft einen Wert ab, der angibt, ob sich die CheckBox im aktivierten Zustand befindet.

```csharp
public bool Checked { get; }
```

### Beispiele

Zeigt, wie man ein PDF generiert, das alle Seiten enthält, die sich auf „Projekt A“ beziehen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Laden Sie das Dokument in Aspose.Note.
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

Zeigt, wie alle Checkbox-Elemente im Zusammenhang mit „Projekt C“ abgeschlossen werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Laden Sie das Dokument in Aspose.Note.
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

Zeigt, wie Sie alle Kontrollkästchen öffnen, die sich auf „Projekt C“ beziehen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Laden Sie das Dokument in Aspose.Note.
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

Zeigt, wie Sie ein PDF generieren, das Seiten mit Elementen enthält, die durch unvollständige Kontrollkästchen markiert und in der letzten Woche erstellt wurden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Laden Sie das Dokument in Aspose.Note.
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

Zeigt, wie Sie eine PDF-Datei generieren, die Seiten mit unvollständigen Outlook-Aufgaben enthält, die in dieser Woche abgeschlossen werden müssen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Laden Sie das Dokument in Aspose.Note.
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

### Siehe auch

* class [CheckBox](../)
* namensraum [Aspose.Note](../../checkbox/)
* Montage [Aspose.Note](../../../)


