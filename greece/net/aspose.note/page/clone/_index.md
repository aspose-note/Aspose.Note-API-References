---
title: Page.Clone
second_title: Aspose.Note for .NET API Reference
description: Page μέθοδος. Κλωνοποιεί τη σελίδα.
type: docs
weight: 140
url: /el/net/aspose.note/page/clone/
---
## Page.Clone method

Κλωνοποιεί τη σελίδα.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| cloneHistory | Boolean | Καθορίζει εάν το ιστορικό της σελίδας πρέπει να κλωνοποιηθεί.. |

### Επιστρεφόμενη Αξία

Ένας κλώνος της σελίδας.

### Παραδείγματα

Δείχνει πώς να προωθήσετε την τρέχουσα έκδοση μιας σελίδας στο ιστορικό.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Δείχνει πώς να κλωνοποιήσετε μια σελίδα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φόρτωση εγγράφου OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Κλωνοποίηση σε νέο έγγραφο χωρίς ιστορικό
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Κλωνοποίηση σε νέο έγγραφο με ιστορικό
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### Δείτε επίσης

* class [Page](../)
* χώρος ονομάτων [Aspose.Note](../../page/)
* συνέλευση [Aspose.Note](../../../)


