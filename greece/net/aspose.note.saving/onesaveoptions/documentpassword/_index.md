---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note for .NET API Reference
description: OneSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης για την κρυπτογράφηση του περιεχομένου του εγγράφου.
type: docs
weight: 20
url: /el/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης για την κρυπτογράφηση του περιεχομένου του εγγράφου.

```csharp
public string DocumentPassword { get; set; }
```

### Παραδείγματα

Δείχνει τον τρόπο αποθήκευσης εγγράφου με κρυπτογράφηση.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### Δείτε επίσης

* class [OneSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../onesaveoptions/)
* συνέλευση [Aspose.Note](../../../)


