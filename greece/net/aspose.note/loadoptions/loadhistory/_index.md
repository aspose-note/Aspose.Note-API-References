---
title: LoadOptions.LoadHistory
second_title: Aspose.Note for .NET API Reference
description: LoadOptions ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η φόρτωση εγγράφων θα πρέπει να αγνοήσει το ιστορικό. Χρησιμοποιήστε αυτήν την επιλογή για να μειώσετε τη χρήση μνήμης και CPU. Η προεπιλεγμένη τιμή είναιαληθής .
type: docs
weight: 30
url: /el/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η φόρτωση εγγράφων θα πρέπει να αγνοήσει το ιστορικό. Χρησιμοποιήστε αυτήν την επιλογή για να μειώσετε τη χρήση μνήμης και CPU. Η προεπιλεγμένη τιμή είναι`αληθής` .

```csharp
public bool LoadHistory { get; set; }
```

### Παραδείγματα

Δείχνει πώς να λαμβάνετε το ιστορικό της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φόρτωση εγγράφου OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Λήψη πρώτης σελίδας
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### Δείτε επίσης

* class [LoadOptions](../)
* χώρος ονομάτων [Aspose.Note](../../loadoptions/)
* συνέλευση [Aspose.Note](../../../)


