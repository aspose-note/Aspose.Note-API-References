---
title: Class NoteTask
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.NoteTask τάξη. Αντιπροσωπεύει μια εργασία σημειώσεων.
type: docs
weight: 400
url: /el/net/aspose.note/notetask/
---
## NoteTask class

Αντιπροσωπεύει μια εργασία σημειώσεων.

```csharp
public sealed class NoteTask : CheckBox, IEquatable<NoteTask>
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Checked](../../aspose.note/checkbox/checked/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν το πλαίσιο ελέγχου είναι σε επιλεγμένη κατάσταση. |
| [CompletedTime](../../aspose.note/checkbox/completedtime/) { get; } | Λαμβάνει ή ορίζει τον χρόνο που ολοκληρώθηκε. |
| [CreationTime](../../aspose.note/checkbox/creationtime/) { get; set; } | Λαμβάνει ή ρυθμίζει το χρόνο δημιουργίας. |
| [DueDate](../../aspose.note/notetask/duedate/) { get; set; } | Λαμβάνει ή ορίζει την ημερομηνία λήξης. |
| override [Icon](../../aspose.note/notetask/icon/) { get; } | Λαμβάνει ή ορίζει το εικονίδιο. |
| [Label](../../aspose.note/checkbox/label/) { get; } | Λαμβάνει το κείμενο της ετικέτας. |
| [Status](../../aspose.note/checkbox/status/) { get; } | Λαμβάνει ή ορίζει την κατάσταση. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| static [CreateCustomFollowUpDate](../../aspose.note/notetask/createcustomfollowupdate/)(DateTime) | Δημιουργεί μια νέα εργασία σημειώσεων με το εικονίδιο NoFollowUpDateFlag και καθορισμένη ημερομηνία λήξης. |
| static [CreateFollowUpNextWeek](../../aspose.note/notetask/createfollowupnextweek/)() | Δημιουργεί μια νέα εργασία σημειώσεων με το εικονίδιο FollowUpNextWeekFlag. |
| static [CreateFollowUpThisWeek](../../aspose.note/notetask/createfollowupthisweek/)() | Δημιουργεί μια νέα εργασία σημειώσεων με το εικονίδιο FollowUpThisWeekFlag. |
| static [CreateFollowUpToday](../../aspose.note/notetask/createfollowuptoday/)() | Δημιουργεί μια νέα εργασία σημειώσεων με το εικονίδιο FollowUpTodayFlag. |
| static [CreateFollowUpTomorrow](../../aspose.note/notetask/createfollowuptomorrow/)() | Δημιουργεί μια νέα εργασία σημειώσεων με το εικονίδιο FollowUpTomorrowFlag. |
| static [CreateNoFollowUpDate](../../aspose.note/notetask/createnofollowupdate/)() | Δημιουργεί μια νέα εργασία σημειώσεων με το εικονίδιο NoFollowUpDateFlag. |
| [Equals](../../aspose.note/notetask/equals/#equals)(NoteTask) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| override [Equals](../../aspose.note/notetask/equals/#equals_1)(object) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| override [GetHashCode](../../aspose.note/notetask/gethashcode/)() | Χρησιμεύει ως συνάρτηση κατακερματισμού για τον τύπο. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)() | Ορίζει την ετικέτα σε κατάσταση ολοκλήρωσης χρησιμοποιώντας την τρέχουσα ώρα ως χρόνο ολοκλήρωσης. |
| [SetCompleted](../../aspose.note/checkbox/setcompleted/)(DateTime) | Ορίζει την ετικέτα σε κατάσταση ολοκληρωμένης. |
| override [SetOpen](../../aspose.note/notetask/setopen/)() | Ορίζει την ετικέτα σε κατάσταση ανοίγματος. |

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

Δείχνει τον τρόπο πρόσβασης σε λεπτομέρειες των εργασιών του Outlook.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tasks();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη όλων των κόμβων RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Επανάληψη σε κάθε κόμβο
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Ανάκτηση ιδιοτήτων
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Δείτε επίσης

* class [CheckBox](../checkbox/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


