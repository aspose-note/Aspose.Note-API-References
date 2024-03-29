---
title: RevisionSummary.LastModifiedTime
second_title: Aspose.Note for .NET API Reference
description: RevisionSummary ιδιοκτησία. Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.
type: docs
weight: 30
url: /el/net/aspose.note/revisionsummary/lastmodifiedtime/
---
## RevisionSummary.LastModifiedTime property

Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Παραδείγματα

Δείχνει πώς να επεξεργαστείτε τις μετα-πληροφορίες της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Ανάγνωση περίληψης αναθεώρησης περιεχομένου για αυτήν τη σελίδα
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Ενημέρωση περίληψης αναθεώρησης σελίδας για αυτήν τη σελίδα
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
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

* class [RevisionSummary](../)
* χώρος ονομάτων [Aspose.Note](../../revisionsummary/)
* συνέλευση [Aspose.Note](../../../)


