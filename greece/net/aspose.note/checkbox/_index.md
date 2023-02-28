---
title: Class CheckBox
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.CheckBox τάξη. Η βασική κλάση για ετικέτες που μπορούν να αλλάξουν την κατάστασή τους μεταξύ πλήρους και ελλιπούς.
type: docs
weight: 20
url: /el/net/aspose.note/checkbox/
---
## CheckBox class

Η βασική κλάση για ετικέτες που μπορούν να αλλάξουν την κατάστασή τους μεταξύ πλήρους και ελλιπούς.

```csharp
public abstract class CheckBox : ITag
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν το πλαίσιο ελέγχου είναι σε επιλεγμένη κατάσταση. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Λαμβάνει ή ορίζει τον χρόνο που ολοκληρώθηκε. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Λαμβάνει ή ρυθμίζει το χρόνο δημιουργίας. |
| abstract [Icon](../../aspose.note/checkbox/icon/) { get; } | Λαμβάνει ή ορίζει το εικονίδιο. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Λαμβάνει το κείμενο της ετικέτας. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Λαμβάνει ή ορίζει την κατάσταση. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted)() | Ορίζει την ετικέτα σε κατάσταση ολοκλήρωσης χρησιμοποιώντας την τρέχουσα ώρα ως χρόνο ολοκλήρωσης. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/#setcompleted_1)(DateTime) | Ορίζει την ετικέτα σε κατάσταση ολοκληρωμένης. |
| virtual [SetOpen](../../aspose.note/checkbox/setopen/)() | Ορίζει την ετικέτα σε κατάσταση ανοίγματος. |

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

* interface [ITag](../itag/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


