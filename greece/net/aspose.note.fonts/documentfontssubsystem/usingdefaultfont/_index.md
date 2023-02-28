---
title: DocumentFontsSubsystem.UsingDefaultFont
second_title: Aspose.Note for .NET API Reference
description: DocumentFontsSubsystem μέθοδος. Δημιουργία νέας παρουσίας DocumentFontsSubsystem χρησιμοποιώντας το καθορισμένο προεπιλεγμένο όνομα γραμματοσειράς.
type: docs
weight: 30
url: /el/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

Δημιουργία νέας παρουσίας DocumentFontsSubsystem χρησιμοποιώντας το καθορισμένο προεπιλεγμένο όνομα γραμματοσειράς.

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontName | String | Το προεπιλεγμένο όνομα γραμματοσειράς. |
| fontsSubstitutions | Dictionary`2 | Οι αντικαταστάσεις γραμματοσειρών. |

### Επιστρεφόμενη Αξία

Το[`DocumentFontsSubsystem`](../) .

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας καθορισμένη προεπιλεγμένη γραμματοσειρά.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

### Δείτε επίσης

* class [DocumentFontsSubsystem](../)
* χώρος ονομάτων [Aspose.Note.Fonts](../../documentfontssubsystem/)
* συνέλευση [Aspose.Note](../../../)


