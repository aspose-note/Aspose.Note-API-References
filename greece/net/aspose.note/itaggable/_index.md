---
title: Interface ITaggable
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.ITaggable διεπαφή. Η διεπαφή για κόμβους που μπορούν να επισημανθούν με ετικέτες.
type: docs
weight: 240
url: /el/net/aspose.note/itaggable/
---
## ITaggable interface

Η διεπαφή για κόμβους που μπορούν να επισημανθούν με ετικέτες.

```csharp
public interface ITaggable : INode
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Tags](../../aspose.note/itaggable/tags/) { get; } | Λαμβάνει τη λίστα με όλες τις ετικέτες. |

### Παραδείγματα

Δείχνει πώς να δημιουργήσετε ένα pdf που περιέχει όλες τις σελίδες που σχετίζονται με το 'Project A'.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Φόρτωση του εγγράφου στο Aspose.Note.
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

Δείχνει πώς να κάνετε ολοκληρωμένα όλα τα στοιχεία του πλαισίου ελέγχου που σχετίζονται με το "Έργο Γ".

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Φόρτωση του εγγράφου στο Aspose.Note.
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

Δείχνει πώς μπορείτε να ανοίξετε όλα τα στοιχεία του πλαισίου ελέγχου που σχετίζονται με το «Έργο Γ».

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Φόρτωση του εγγράφου στο Aspose.Note.
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

Δείχνει πώς να δημιουργήσετε ένα pdf που περιέχει σελίδες με στοιχεία που επισημαίνονται με ελλιπή πλαίσια ελέγχου και δημιουργήθηκαν την προηγούμενη εβδομάδα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Φόρτωση του εγγράφου στο Aspose.Note.
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

Δείχνει πώς να δημιουργήσετε ένα pdf που περιέχει σελίδες με ημιτελείς εργασίες του Outlook που πρέπει να ολοκληρώσετε αυτήν την εβδομάδα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Φόρτωση του εγγράφου στο Aspose.Note.
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

### Δείτε επίσης

* interface [INode](../inode/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


