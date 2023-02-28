---
title: Class HtmlSaveOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.HtmlSaveOptions τάξη. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του εγγράφου σε μορφή HTML.
type: docs
weight: 700
url: /el/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του εγγράφου σε μορφή HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | Λαμβάνει ή ορίζει εάν το αρχείο StyleSheet θα δημιουργηθεί για κάθε νέα σελίδα ξεχωριστά. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Λαμβάνει ή ορίζει την επιστροφή κλήσης που καλείται για τη δημιουργία πόρου για αποθήκευση CSS. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν είναι ενεργοποιημένο το έγγραφο ανά δημιουργία σελίδας. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | Λαμβάνει ή ορίζει τον τρόπο εξαγωγής του css. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των γραμματοσειρών. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των εικόνων. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Λαμβάνει ή ορίζει τους τύπους όψεων γραμματοσειράς. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Λαμβάνει ή ορίζει την επανάκληση που καλείται να δημιουργήσει πόρο για αποθήκευση γραμματοσειράς. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Λαμβάνει ή ορίζει τις ρυθμίσεις της γραμματοσειράς που θα χρησιμοποιηθούν κατά την αποθήκευση |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Λαμβάνει ή ορίζει την επανάκληση που καλείται να δημιουργήσει πόρο για αποθήκευση εικόνας. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των σελίδων προς αποθήκευση. Από προεπιλογή είναιMaxValue που σημαίνει ότι όλες οι σελίδες του εγγράφου θα αποδοθούν. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Λαμβάνει ή ορίζει το ευρετήριο της πρώτης σελίδας προς αποθήκευση. Από προεπιλογή είναι 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Λαμβάνει ή ορίζει την επιστροφή κλήσης που καλείται να δημιουργήσει πόρο για αποθήκευση σελίδας. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Λαμβάνει τη μορφή στην οποία είναι αποθηκευμένο το έγγραφο. |

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή html με την αποθήκευση όλων των πόρων (css/fonts/εικόνες) σε ξεχωριστά αρχεία.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

Δείχνει τον τρόπο αποθήκευσης ενός εγγράφου σε ροή σε μορφή html με ενσωμάτωση όλων των πόρων (css/fonts/images).

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
```

Δείχνει πώς να δημιουργήσετε ένα έγγραφο και να αποθηκεύσετε σε μορφή html το καθορισμένο εύρος σελίδων.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Εκκίνηση εγγράφου OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Προεπιλεγμένο στυλ για όλο το κείμενο του εγγράφου.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Αποθήκευση σε μορφή HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή html με την αποθήκευση όλων των πόρων (css/ γραμματοσειρές/εικόνες) χρησιμοποιώντας επανακλήσεις που ορίζονται από το χρήστη.

```csharp
// Ο παρακάτω κώδικας δημιουργεί φάκελο "documentFolder" που περιέχει document.html, φάκελο "css" με αρχείο "style.css", φάκελο "images" με εικόνες και φάκελο "fonts" με γραμματοσειρές.
// Το αρχείο 'style.css' θα περιέχει στο τέλος την ακόλουθη συμβολοσειρά "/* Αυτή η γραμμή προστίθεται στη ροή μη αυτόματα από τον χρήστη */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

### Δείτε επίσης

* class [SaveOptions](../saveoptions/)
* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


