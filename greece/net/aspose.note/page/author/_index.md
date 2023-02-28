---
title: Page.Author
second_title: Aspose.Note for .NET API Reference
description: Page ιδιοκτησία. Λαμβάνει ή ορίζει τον συγγραφέα.
type: docs
weight: 20
url: /el/net/aspose.note/page/author/
---
## Page.Author property

Λαμβάνει ή ορίζει τον συγγραφέα.

```csharp
public string Author { get; set; }
```

### Παραδείγματα

Δείχνει πώς να λαμβάνετε μετα-πληροφορίες για μια σελίδα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
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

* class [Page](../)
* χώρος ονομάτων [Aspose.Note](../../page/)
* συνέλευση [Aspose.Note](../../../)


