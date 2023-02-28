---
title: Document.GetPageHistory
second_title: Aspose.Note for .NET API Reference
description: Document μέθοδος. Λαμβάνει τοPageHistory που περιέχει πλήρες ιστορικό για κάθε σελίδα που παρουσιάζεται σε ένα έγγραφο το παλαιότερο στο ευρετήριο 0. Η τρέχουσα αναθεώρηση σελίδας μπορεί να προσπελαστεί ωςCurrent και περιέχεται χωριστά από τη συλλογή ιστορικών εκδόσεων.
type: docs
weight: 100
url: /el/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

Λαμβάνει το[`PageHistory`](../../pagehistory/) που περιέχει πλήρες ιστορικό για κάθε σελίδα που παρουσιάζεται σε ένα έγγραφο (το παλαιότερο στο ευρετήριο 0). Η τρέχουσα αναθεώρηση σελίδας μπορεί να προσπελαστεί ως[`Current`](../../pagehistory/current/) και περιέχεται χωριστά από τη συλλογή ιστορικών εκδόσεων.

```csharp
public PageHistory GetPageHistory(Page page)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| page | Page | Η τρέχουσα αναθεώρηση μιας σελίδας. |

### Επιστρεφόμενη Αξία

Το[`PageHistory`](../../pagehistory/) .

### Παραδείγματα

Δείχνει πώς να επαναφέρετε την προηγούμενη έκδοση μιας σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Δείχνει πώς να επεξεργαστείτε το ιστορικό της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

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

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


