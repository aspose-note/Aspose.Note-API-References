---
title: Class CheckBox
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.CheckBox klas. Die Basisklasse für Tags die ihren Zustand zwischen vollständig und unvollständig umschalten können.
type: docs
weight: 20
url: /de/net/aspose.note/checkbox/
---
## CheckBox class

Die Basisklasse für Tags, die ihren Zustand zwischen vollständig und unvollständig umschalten können.

```csharp
public abstract class CheckBox : ITag
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Ruft einen Wert ab, der angibt, ob sich die CheckBox im aktivierten Zustand befindet. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Ruft die abgeschlossene Zeit ab oder legt sie fest. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Ruft die Erstellungszeit ab oder legt sie fest. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | Ruft das Symbol ab oder legt es fest. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Ruft den Beschriftungstext ab. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Ruft den Status ab oder setzt ihn. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | Versetzt das Tag in den abgeschlossenen Zustand, wobei die aktuelle Zeit als abgeschlossene Zeit verwendet wird. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | Versetzt das Tag in den abgeschlossenen Zustand. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | Versetzt das Tag in den offenen Zustand. |

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

* interface [ITag](../itag/)
* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


