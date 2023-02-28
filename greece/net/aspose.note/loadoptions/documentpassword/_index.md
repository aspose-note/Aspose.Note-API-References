---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note for .NET API Reference
description: LoadOptions ιδιοκτησία. Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης για το κρυπτογραφημένο περιεχόμενο του εγγράφου. Η τιμή αγνοείται σε περίπτωση που το έγγραφο δεν προστατεύεται με κωδικό πρόσβασης.
type: docs
weight: 20
url: /el/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης για το κρυπτογραφημένο περιεχόμενο του εγγράφου. Η τιμή αγνοείται σε περίπτωση που το έγγραφο δεν προστατεύεται με κωδικό πρόσβασης.

```csharp
public string DocumentPassword { get; set; }
```

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

### Δείτε επίσης

* class [LoadOptions](../)
* χώρος ονομάτων [Aspose.Note](../../loadoptions/)
* συνέλευση [Aspose.Note](../../../)


