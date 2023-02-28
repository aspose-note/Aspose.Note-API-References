---
title: Class LoadOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.LoadOptions τάξη. Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός εγγράφου.
type: docs
weight: 320
url: /el/net/aspose.note/loadoptions/
---
## LoadOptions class

Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός εγγράφου.

```csharp
public class LoadOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [LoadOptions](loadoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης για το κρυπτογραφημένο περιεχόμενο του εγγράφου. Η τιμή αγνοείται σε περίπτωση που το έγγραφο δεν προστατεύεται με κωδικό πρόσβασης. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η φόρτωση εγγράφων θα πρέπει να αγνοήσει το ιστορικό. Χρησιμοποιήστε αυτήν την επιλογή για να μειώσετε τη χρήση μνήμης και CPU. Η προεπιλεγμένη τιμή είναι`αληθής` . |

### Παραδείγματα

Δείχνει τον τρόπο δημιουργίας κρυπτογραφημένου εγγράφου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Δείχνει πώς να κάνετε ένα κρυπτογραφημένο σημειωματάριο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

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

* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


