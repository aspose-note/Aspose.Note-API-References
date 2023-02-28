---
title: CompositeNode1.FirstChild
second_title: Aspose.Note for .NET API Reference
description: CompositeNode ιδιοκτησία. Λαμβάνει τον πρώτο θυγατρικό κόμβο αυτού του κόμβου.
type: docs
weight: 10
url: /el/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

Λαμβάνει τον πρώτο θυγατρικό κόμβο αυτού του κόμβου.

```csharp
public T FirstChild { get; }
```

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

* class [CompositeNode&lt;T&gt;](../)
* χώρος ονομάτων [Aspose.Note](../../compositenode-1/)
* συνέλευση [Aspose.Note](../../../)


