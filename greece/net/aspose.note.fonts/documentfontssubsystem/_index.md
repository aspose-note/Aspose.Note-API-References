---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Fonts.DocumentFontsSubsystem τάξη. Απλή υλοποίηση του Aspose.Note.Fonts.FontsSubsystem. ΑνάκτησηFontFamily αντικείμενο από το OS.
type: docs
weight: 100
url: /el/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Απλή υλοποίηση του Aspose.Note.Fonts.FontsSubsystem. ΑνάκτησηFontFamily αντικείμενο από το OS.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | Αρχικοποιεί μια νέα παρουσία του`DocumentFontsSubsystem` τάξη. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Αρχικοποιεί μια νέα παρουσία του`DocumentFontsSubsystem` τάξη. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | Αρχικοποιεί μια νέα παρουσία του`DocumentFontsSubsystem` τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | Λαμβάνει ή ορίζει το στατικό προεπιλεγμένο στιγμιότυπο. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Λαμβάνει ή ορίζει την προεπιλεγμένη γραμματοσειρά. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | Δημιουργία νέας παρουσίας DocumentFontsSubsystem χρησιμοποιώντας το καθορισμένο προεπιλεγμένο όνομα γραμματοσειράς. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | Δημιουργία νέας παρουσίας DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από καθορισμένο αρχείο ως προεπιλογή. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | Δημιουργία νέας παρουσίας DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από καθορισμένη ροή ως προεπιλογή. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | Προσθέστε τη γραμματοσειρά. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | Προσθέστε τη γραμματοσειρά. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | Προσθέστε τη γραμματοσειρά. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Προσθέτει αντικατάσταση γραμματοσειράς. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Αποκτά οικογένεια γραμματοσειρών. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Φορτώνει όλες τις γραμματοσειρές TrueType από τον καθορισμένο φάκελο στην εσωτερική συλλογή. |

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

* class [FontsSubsystem](../fontssubsystem/)
* χώρος ονομάτων [Aspose.Note.Fonts](../../aspose.note.fonts/)
* συνέλευση [Aspose.Note](../../)


