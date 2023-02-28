---
title: Class OneSaveOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.OneSaveOptions τάξη. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση εγγράφου σε μορφή OneNote.
type: docs
weight: 810
url: /el/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση εγγράφου σε μορφή OneNote.

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης για την κρυπτογράφηση του περιεχομένου του εγγράφου. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Λαμβάνει ή ορίζει τις ρυθμίσεις της γραμματοσειράς που θα χρησιμοποιηθούν κατά την αποθήκευση |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των σελίδων προς αποθήκευση. Από προεπιλογή είναιMaxValue που σημαίνει ότι όλες οι σελίδες του εγγράφου θα αποδοθούν. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Λαμβάνει ή ορίζει το ευρετήριο της πρώτης σελίδας προς αποθήκευση. Από προεπιλογή είναι 0. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Λαμβάνει τη μορφή στην οποία είναι αποθηκευμένο το έγγραφο. |

### Παραδείγματα

Δείχνει τον τρόπο αποθήκευσης εγγράφου με κρυπτογράφηση.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο χρησιμοποιώντας το OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### Δείτε επίσης

* class [SaveOptions](../saveoptions/)
* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


