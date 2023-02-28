---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note for .NET API Reference
description: NotebookLoadOptions ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα παιδικά έγγραφα θα πρέπει να φορτωθούν ρητά αργότερα.
type: docs
weight: 20
url: /el/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα παιδικά έγγραφα θα πρέπει να φορτωθούν ρητά αργότερα.

```csharp
public bool DeferredLoading { get; set; }
```

### Παρατηρήσεις

Η προεπιλεγμένη τιμή είναι`ψευδής` , επομένως τα θυγατρικά έγγραφα θα φορτωθούν σιωπηρά. Τιμή`αληθής` υποδεικνύει ότι ο χρήστης πρέπει να καλέσει[`LoadChildDocument`](../../notebook/loadchilddocument/) ή για τον θυγατρικό κόμβο κάθε σημειωματάριου μετά τη φόρτωση του ίδιου του σημειωματάριου. Εάν η τιμή είναι`αληθής` ,[`InstantLoading`](../instantloading/) Η επιλογή θα αγνοηθεί. Εάν ο φορητός υπολογιστής φορτώνεται από τη ροή, η τιμή είναι πάντα`αληθής` παρότι ορίστηκε ρητά από τον χρήστη σε`ψευδής` .

### Παραδείγματα

Δείχνει πώς να κάνετε ένα κρυπτογραφημένο σημειωματάριο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### Δείτε επίσης

* class [NotebookLoadOptions](../)
* χώρος ονομάτων [Aspose.Note](../../notebookloadoptions/)
* συνέλευση [Aspose.Note](../../../)


