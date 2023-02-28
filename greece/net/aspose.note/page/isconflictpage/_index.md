---
title: Page.IsConflictPage
second_title: Aspose.Note for .NET API Reference
description: Page ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν αυτή η σελίδα είναι σελίδα διένεξης.
type: docs
weight: 50
url: /el/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν αυτή η σελίδα είναι σελίδα διένεξης.

```csharp
public bool IsConflictPage { get; set; }
```

### Παρατηρήσεις

Η σελίδα διένεξης προκύπτει όταν δύο χρήστες προσπαθούν να ενημερώσουν το ίδιο περιεχόμενο. Σε αυτήν την περίπτωση οι αλλαγές του πρώτου χρήστη γράφονται ως συνήθως. Αλλά οι αλλαγές ενός άλλου χρήστη δεν μπορούν να συγχωνευθούν. Έτσι δημιουργείται απλώς ένα αντίγραφο της σελίδας και επισημάνθηκε ως διένεξη.

Σε αυτήν την έκδοση, οι διενέξεις επιλύονται υπέρ των αλλαγών του πρώτου χρήστη. Επομένως, εάν το έγγραφο έχει σελίδες διένεξης, τότε αυτές θα εμφανίζονται στο ιστορικό αλλά θα παραβλεφθούν κατά την αποθήκευση. Είναι δυνατή η επαναφορά αυτής της σημαίας για αποθήκευση αυτής της σελίδας στην ιστορία ως συνήθως.

Λεπτομερές δείγμα χειρισμού κατά σελίδα διένεξης μπορείτε να βρείτε στην ηλεκτρονική τεκμηρίωση.

### Παραδείγματα

Δείχνει πώς μπορείτε να ελέγξετε εάν μια σελίδα είναι σελίδα διένεξης (δηλ. έχει αλλαγές που το OneNote δεν μπορούσε να συγχωνεύσει αυτόματα).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Φόρτωση εγγράφου OneNote
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Από προεπιλογή, οι σελίδες διένεξης απλώς παραλείπονται κατά την αποθήκευση.
    // Εάν το επισημάνετε ως μη σύγκρουση, τότε θα αποθηκευτεί ως συνήθως στο ιστορικό.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Δείτε επίσης

* class [Page](../)
* χώρος ονομάτων [Aspose.Note](../../page/)
* συνέλευση [Aspose.Note](../../../)


