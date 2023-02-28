---
title: ImageSaveOptions.Resolution
second_title: Aspose.Note for .NET API Reference
description: ImageSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει την ανάλυση για τις εικόνες που δημιουργούνται σε κουκκίδες ανά ίντσα.
type: docs
weight: 50
url: /el/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

Λαμβάνει ή ορίζει την ανάλυση για τις εικόνες που δημιουργούνται, σε κουκκίδες ανά ίντσα.

```csharp
public float Resolution { get; set; }
```

### Παρατηρήσεις

Η προεπιλεγμένη τιμή είναι 96.

### Παραδείγματα

Δείχνει πώς να ορίσετε μια ανάλυση εικόνας κατά την αποθήκευση εγγράφου ως εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Αποθηκεύστε το έγγραφο.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Δείχνει πώς να αποθηκεύσετε το σημειωματάριο ως εικόνα με καθορισμένες επιλογές.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir, notebookSaveOptions);
```

Δείχνει πώς να αποθηκεύσετε το πεπλατυσμένο σημειωματάριο ως εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir, notebookSaveOptions);
```

### Δείτε επίσης

* class [ImageSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../imagesaveoptions/)
* συνέλευση [Aspose.Note](../../../)


