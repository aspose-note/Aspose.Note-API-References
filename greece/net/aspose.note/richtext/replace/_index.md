---
title: RichText.Replace
second_title: Aspose.Note for .NET API Reference
description: RichText μέθοδος. Αντικαθιστά όλες τις εμφανίσεις ενός καθορισμένου χαρακτήρα Unicode σε αυτήν την περίπτωση με έναν άλλο καθορισμένο χαρακτήρα Unicode.
type: docs
weight: 200
url: /el/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

Αντικαθιστά όλες τις εμφανίσεις ενός καθορισμένου χαρακτήρα Unicode σε αυτήν την περίπτωση με έναν άλλο καθορισμένο χαρακτήρα Unicode.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldChar | Char | Το παλιό χαρ. |
| newChar | Char | Το νέο χαρ. |

### Επιστρεφόμενη Αξία

Το[`RichText`](../) .

### Δείτε επίσης

* class [RichText](../)
* χώρος ονομάτων [Aspose.Note](../../richtext/)
* συνέλευση [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία με μια άλλη καθορισμένη συμβολοσειρά.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldValue | String | Η παλιά τιμή. |
| newValue | String | Η νέα τιμή. |

### Επιστρεφόμενη Αξία

Το[`RichText`](../) .

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Παραδείγματα

Δείχνει πώς να περάσετε μέσα από το κείμενο της σελίδας και να κάνετε μια αντικατάσταση.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Λήψη όλων των κόμβων RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Αντικατάσταση κειμένου σχήματος
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Αποθήκευση σε οποιαδήποτε υποστηριζόμενη μορφή αρχείου
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Δείχνει πώς να δημιουργήσετε ένα νέο έγγραφο αντικαθιστώντας ειδικά κομμάτια κειμένου σε ένα πρότυπο.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// Φόρτωση του προτύπου εγγράφου στο Aspose.Note.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// Ας αντικαταστήσουμε όλες τις λέξεις προτύπου
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### Δείτε επίσης

* class [RichText](../)
* χώρος ονομάτων [Aspose.Note](../../richtext/)
* συνέλευση [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία με μια άλλη καθορισμένη συμβολοσειρά σε καθορισμένο στυλ.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldValue | String | Η παλιά τιμή. |
| newValue | String | Η νέα τιμή. |
| style | TextStyle | Το στυλ της νέας τιμής. |

### Επιστρεφόμενη Αξία

Το[`RichText`](../) .

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Δείτε επίσης

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* χώρος ονομάτων [Aspose.Note](../../richtext/)
* συνέλευση [Aspose.Note](../../../)


