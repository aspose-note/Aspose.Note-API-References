---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note for .NET API Reference
description: DocumentFontsSubsystem μέθοδος. Δημιουργία νέας παρουσίας DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από καθορισμένο αρχείο ως προεπιλογή.
type: docs
weight: 40
url: /el/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

Δημιουργία νέας παρουσίας DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από καθορισμένο αρχείο ως προεπιλογή.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Το αρχείο που περιέχει το προεπιλεγμένο όνομα γραμματοσειράς. |
| fontsSubstitutions | Dictionary`2 | Οι αντικαταστάσεις γραμματοσειρών. |

### Επιστρεφόμενη Αξία

Το[`DocumentFontsSubsystem`](../) .

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας την προεπιλεγμένη γραμματοσειρά από ένα αρχείο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

### Δείτε επίσης

* class [DocumentFontsSubsystem](../)
* χώρος ονομάτων [Aspose.Note.Fonts](../../documentfontssubsystem/)
* συνέλευση [Aspose.Note](../../../)


