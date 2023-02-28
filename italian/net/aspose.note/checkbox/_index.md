---
title: Class CheckBox
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.CheckBox classe. La classe base per i tag che possono alternare il proprio stato tra completo e incompleto.
type: docs
weight: 20
url: /it/net/aspose.note/checkbox/
---
## CheckBox class

La classe base per i tag che possono alternare il proprio stato tra completo e incompleto.

```csharp
public abstract class CheckBox : ITag
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Ottiene un valore che indica se CheckBox è nello stato selezionato. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Ottiene o imposta il tempo di completamento. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Ottiene o imposta l'ora di creazione. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | Ottiene o imposta l'icona. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Ottiene il testo dell'etichetta. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Ottiene o imposta lo stato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | Imposta il tag sullo stato completato utilizzando l'ora corrente come ora completata. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | Imposta il tag sullo stato completato. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | Imposta il tag sullo stato aperto. |

### Esempi

Mostra come generare un pdf contenente tutte le pagine relative al 'Progetto A'.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
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

Mostra come completare tutti gli elementi della casella di controllo relativi al "Progetto C".

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
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

Mostra come aprire tutti gli elementi della casella di controllo relativi al "Progetto C".

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
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

Mostra come generare un pdf contenente pagine con elementi contrassegnati da caselle di controllo incomplete e creati durante la scorsa settimana.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
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

Mostra come generare un pdf contenente pagine con attività incomplete di Outlook da completare questa settimana.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
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

### Guarda anche

* interface [ITag](../itag/)
* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


