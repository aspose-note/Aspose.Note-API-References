---
title: CheckBox.SetCompleted
second_title: Aspose.Note for .NET API Reference
description: CheckBox μέθοδος. Ορίζει την ετικέτα σε κατάσταση ολοκληρωμένης.
type: docs
weight: 70
url: /el/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

Ορίζει την ετικέτα σε κατάσταση ολοκληρωμένης.

```csharp
public void SetCompleted(DateTime completedTime)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| completedTime | DateTime | Ο χρόνος που ολοκληρώθηκε. |

### Δείτε επίσης

* class [CheckBox](../)
* χώρος ονομάτων [Aspose.Note](../../checkbox/)
* συνέλευση [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

Ορίζει την ετικέτα σε κατάσταση ολοκλήρωσης χρησιμοποιώντας την τρέχουσα ώρα ως χρόνο ολοκλήρωσης.

```csharp
public void SetCompleted()
```

### Παραδείγματα

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

### Δείτε επίσης

* class [CheckBox](../)
* χώρος ονομάτων [Aspose.Note](../../checkbox/)
* συνέλευση [Aspose.Note](../../../)


