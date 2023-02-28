---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note for .NET API Reference
description: DocumentFontsSubsystem μέθοδος. Δημιουργία νέας παρουσίας DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από καθορισμένη ροή ως προεπιλογή.
type: docs
weight: 50
url: /el/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Δημιουργία νέας παρουσίας DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από καθορισμένη ροή ως προεπιλογή.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontStream | Stream | Η ροή που περιέχει το προεπιλεγμένο όνομα γραμματοσειράς. |
| fontsSubstitutions | Dictionary`2 | Οι αντικαταστάσεις γραμματοσειρών. |

### Επιστρεφόμενη Αξία

Το[`DocumentFontsSubsystem`](../) .

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας προεπιλεγμένη γραμματοσειρά από μια ροή.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Δείτε επίσης

* class [DocumentFontsSubsystem](../)
* χώρος ονομάτων [Aspose.Note.Fonts](../../documentfontssubsystem/)
* συνέλευση [Aspose.Note](../../../)


