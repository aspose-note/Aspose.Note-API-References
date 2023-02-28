---
title: Class Document
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Document τάξη. Αντιπροσωπεύει ένα έγγραφο Aspose.Note.
type: docs
weight: 60
url: /el/net/aspose.note/document/
---
## Document class

Αντιπροσωπεύει ένα έγγραφο Aspose.Note.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [Document](document/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`Document` class. Δημιουργεί ένα κενό έγγραφο OneNote. |
| [Document](document/#constructor_1)(Stream) | Αρχικοποιεί μια νέα παρουσία του`Document` class. Ανοίγει ένα υπάρχον έγγραφο OneNote από μια ροή. |
| [Document](document/#constructor_3)(string) | Αρχικοποιεί μια νέα παρουσία του`Document` class. Ανοίγει ένα υπάρχον έγγραφο OneNote από ένα αρχείο. |
| [Document](document/#constructor_2)(Stream, LoadOptions) | Αρχικοποιεί μια νέα παρουσία του`Document` class. Ανοίγει ένα υπάρχον έγγραφο OneNote από μια ροή. Επιτρέπει τον καθορισμό πρόσθετων επιλογών, όπως έναν κωδικό πρόσβασης κρυπτογράφησης. |
| [Document](document/#constructor_4)(string, LoadOptions) | Αρχικοποιεί μια νέα παρουσία του`Document`class. Ανοίγει ένα υπάρχον έγγραφο του OneNote από ένα αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών, όπως έναν κωδικό πρόσβασης κρυπτογράφησης. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το Aspose.Note εκτελεί αυτόματα τον εντοπισμό αλλαγών διάταξης. Η προεπιλεγμένη τιμή είναι`αληθής` . |
| [Color](../../aspose.note/document/color/) { get; set; } | Παίρνει ή ρυθμίζει το χρώμα. |
| [CreationTime](../../aspose.note/document/creationtime/) { get; set; } | Λαμβάνει ή ρυθμίζει το χρόνο δημιουργίας. |
| [DisplayName](../../aspose.note/document/displayname/) { get; set; } | Λαμβάνει ή ορίζει το εμφανιζόμενο όνομα. |
| [Document](../../aspose.note/node/document/) { get; } | Λαμβάνει το έγγραφο του κόμβου. |
| [FileFormat](../../aspose.note/document/fileformat/) { get; } | Λαμβάνει μορφή αρχείου (OneNote 2010, OneNote Online). |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Guid](../../aspose.note/document/guid/) { get; } | Λαμβάνει το παγκοσμίως μοναδικό αναγνωριστικό του αντικειμένου. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Λαμβάνει τον επόμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Παίρνει τον τύπο κόμβου. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Λαμβάνει τον γονικό κόμβο. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Λαμβάνει τον προηγούμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [Accept](../../aspose.note/document/accept/)(DocumentVisitor) | Αποδέχεται τον επισκέπτη του κόμβου. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges/)() | Ανιχνεύει όλες τις αλλαγές που έγιναν στη διάταξη του εγγράφου από την προηγούμενη[`DetectLayoutChanges`](./detectlayoutchanges/) καλέστε. Σε περίπτωση[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled/) ορίστηκε σε true, χρησιμοποιείται αυτόματα στην αρχή της εξαγωγής εγγράφου. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory/)(Page) | Λαμβάνει το[`PageHistory`](../pagehistory/) που περιέχει πλήρες ιστορικό για κάθε σελίδα που παρουσιάζεται σε ένα έγγραφο (το παλαιότερο στο ευρετήριο 0). Η τρέχουσα αναθεώρηση σελίδας μπορεί να προσπελαστεί ως[`Current`](../pagehistory/current/) και περιέχεται χωριστά από τη συλλογή ιστορικών εκδόσεων. |
| [Import](../../aspose.note/document/import/#import)(Stream, PdfImportOptions, MergeOptions) | Εισάγει ένα σύνολο σελίδων από το παρεχόμενο έγγραφο PDF. |
| [Import](../../aspose.note/document/import/#import_1)(string, PdfImportOptions, MergeOptions) | Εισάγει ένα σύνολο σελίδων από το παρεχόμενο έγγραφο PDF. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge/)(IEnumerable&lt;Page&gt;, MergeOptions) | Συγχωνεύει ένα σύνολο σελίδων στο έγγραφο. |
| [Print](../../aspose.note/document/print/#print)() | Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή. |
| [Print](../../aspose.note/document/print/#print_1)(PrintOptions) | Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Save](../../aspose.note/document/save/#save)(Stream) | Αποθηκεύει το έγγραφο του OneNote σε μια ροή. |
| [Save](../../aspose.note/document/save/#save_3)(string) | Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο. |
| [Save](../../aspose.note/document/save/#save_1)(Stream, SaveFormat) | Αποθηκεύει το έγγραφο του OneNote σε μια ροή με την καθορισμένη μορφή. |
| [Save](../../aspose.note/document/save/#save_2)(Stream, SaveOptions) | Αποθηκεύει το έγγραφο του OneNote σε μια ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [Save](../../aspose.note/document/save/#save_4)(string, SaveFormat) | Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο στην καθορισμένη μορφή. |
| [Save](../../aspose.note/document/save/#save_5)(string, SaveOptions) | Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted)(Stream, out Document) | Ελέγχει εάν ένα έγγραφο από μια ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_3)(string, out Document) | Ελέγχει εάν ένα έγγραφο από ένα αρχείο είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_1)(Stream, LoadOptions, out Document) | Ελέγχει εάν ένα έγγραφο από μια ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_2)(Stream, string, out Document) | Ελέγχει εάν ένα έγγραφο από μια ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_4)(string, LoadOptions, out Document) | Ελέγχει εάν ένα έγγραφο από ένα αρχείο είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_5)(string, string, out Document) | Ελέγχει εάν ένα έγγραφο από ένα αρχείο είναι κρυπτογραφημένο. Για να το ελέγξουμε πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Επομένως, αυτή η μέθοδος μπορεί να οδηγήσει σε ποινή απόδοσης. |

### Παραδείγματα

Δείχνει τον τρόπο αποστολής εγγράφου σε εκτυπωτή χρησιμοποιώντας τυπικό παράθυρο διαλόγου των Windows με προεπιλεγμένες επιλογές.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

Δείχνει τον τρόπο δημιουργίας κρυπτογραφημένου εγγράφου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

Δείχνει τον τρόπο αποθήκευσης εγγράφου με κρυπτογράφηση.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο χρησιμοποιώντας την απαρίθμηση SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο χρησιμοποιώντας το OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

Δείχνει πώς να λαμβάνετε τον αριθμό της σελίδας ενός εγγράφου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη αριθμού σελίδων
int count = oneFile.Count();

// Αριθμός εκτυπώσεων στην οθόνη εξόδου
Console.WriteLine(count);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας τις προεπιλεγμένες ρυθμίσεις.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή gif.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Αποθηκεύστε το έγγραφο ως gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Δείχνει πώς να ορίσετε μια ποιότητα εικόνας κατά την αποθήκευση εγγράφου ως εικόνα σε μορφή JPEG.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Αποθηκεύστε το έγγραφο.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

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

Δείχνει πώς να αποκτήσετε τη μορφή αρχείου ενός εγγράφου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Process OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Επεξεργαστείτε το OneNote Online
        break;
}
```

Δείχνει πώς να συνδέσετε μια υπερσύνδεση σε μια εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μια ροή.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Επανατύλιξη της θέσης ροής πίσω στο μηδέν, ώστε να είναι έτοιμη για την επόμενη ανάγνωση.
dstStream.Seek(0, SeekOrigin.Begin);
```

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Δείχνει πώς να προσθέσετε νέα ενότητα σε ένα σημειωματάριο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Προσθήκη νέου παιδιού στο Σημειωματάριο
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir);
```

Δείχνει πώς μπορείτε να ελέγξετε εάν η φόρτωση ενός εγγράφου απέτυχε επειδή δεν υποστηρίζεται η μορφή OneNote 2007.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

Δείχνει πώς να επαναφέρετε την προηγούμενη έκδοση μιας σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Δείχνει πώς να κλωνοποιήσετε μια σελίδα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φόρτωση εγγράφου OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Κλωνοποίηση σε νέο έγγραφο χωρίς ιστορικό
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Κλωνοποίηση σε νέο έγγραφο με ιστορικό
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

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

Δείχνει πώς να ορίσετε την περιγραφή κειμένου για μια εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

Δείχνει πώς να λαμβάνετε μετα-πληροφορίες για μια σελίδα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

Όταν οι μεγάλες σελίδες του OneNote αποθηκεύονται σε μορφή pdf, χωρίζονται σε σελίδες. Το δείγμα δείχνει πώς να διαμορφώσετε τη λογική διαχωρισμού των αντικειμένων που βρίσκονται στα διαλείμματα της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή png.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Εκκίνηση αντικειμένου ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Ορισμός ευρετηρίου σελίδας
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Αποθηκεύστε το έγγραφο ως PNG.
oneFile.Save(dataDir, opts);
```

Δείχνει πώς να επεξεργαστείτε το ιστορικό της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Δείχνει πώς μπορείτε να ελέγξετε εάν ένα έγγραφο προστατεύεται με κωδικό πρόσβασης με συγκεκριμένο κωδικό πρόσβασης.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

Δείχνει πώς να εφαρμόσετε το στυλ σκούρου θέματος σε ένα έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

Δείχνει πώς να περάσει μέσα από το περιεχόμενο ενός σημειωματάριου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // Κάντε κάτι με το θυγατρικό έγγραφο
        }
        else if (notebookChildNode is Notebook)
        {
            // Κάντε κάτι με το παιδικό σημειωματάριο
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

Δείχνει πώς να λάβετε μια εικόνα από ένα έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη όλων των κόμβων εικόνας
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Αποθήκευση byte εικόνας σε ένα αρχείο
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Αρχικοποίηση αντικειμένου PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Ορισμός ευρετηρίου σελίδας της πρώτης σελίδας που θα αποθηκευτεί
                              PageIndex = 0,

                              // Ορισμός αριθμού σελίδων
                              PageCount = 1,
                          };

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας συγκεκριμένες ρυθμίσεις.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Αρχικοποίηση αντικειμένου PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Χρησιμοποιήστε συμπίεση Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Ποιότητα για συμπίεση JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Δείχνει τον τρόπο αποστολής εγγράφου σε εκτυπωτή χρησιμοποιώντας τυπικό παράθυρο διαλόγου των Windows με καθορισμένες επιλογές.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

Δείχνει τον τρόπο λήψης περιεχομένου ενός συνημμένου αρχείου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Attachments();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Λάβετε μια λίστα με συνημμένους κόμβους αρχείων
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Επανάληψη σε όλους τους κόμβους
foreach (AttachedFile file in nodes)
{
    // Φόρτωση συνημμένου αρχείου σε αντικείμενο ροής
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Δημιουργία τοπικού αρχείου
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Αντιγραφή ροής αρχείου
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Δείχνει πώς να λαμβάνετε μετα-πληροφορίες εικόνας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη όλων των κόμβων εικόνας
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

Δείχνει πώς να λαμβάνετε το ιστορικό της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φόρτωση εγγράφου OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Λήψη πρώτης σελίδας
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

Δείχνει πώς να προσθέσετε ένα αρχείο σε ένα έγγραφο χρησιμοποιώντας τη διαδρομή αρχείου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Attachments();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης Outline
Outline outline = new Outline(doc);

// Αρχικοποίηση αντικειμένου κλάσης OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Αρχικοποίηση αντικειμένου κλάσης AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Προσθήκη συνημμένου αρχείου
outlineElem.AppendChildLast(attachedFile);

// Προσθήκη κόμβου στοιχείου περιγράμματος
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου περιγράμματος
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Δείχνει πώς να δημιουργήσετε ένα έγγραφο και να το αποθηκεύσετε σε μορφή html χρησιμοποιώντας τις προεπιλεγμένες επιλογές.

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
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Δείχνει πώς μπορείτε να ελέγξετε εάν μια σελίδα είναι σελίδα διένεξης (δηλ. έχει αλλαγές που το OneNote δεν μπορούσε να συγχωνεύσει αυτόματα).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Φόρτωση εγγράφου OneNote
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Από προεπιλογή, οι σελίδες διένεξης απλώς παραλείπονται κατά την αποθήκευση.
    // Εάν το επισημάνετε ως μη σύγκρουση, τότε θα αποθηκευτεί ως συνήθως στο ιστορικό.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

Δείχνει πώς να προσθέσετε μια εικόνα από αρχείο σε έγγραφο με ιδιότητες καθορισμένες από το χρήστη.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Φόρτωση εγγράφου από τη ροή.
Document doc = new Document(dataDir + "Aspose.one");

// Λάβετε την πρώτη σελίδα του εγγράφου.
Aspose.Note.Page page = doc.FirstChild;

// Φόρτωση εικόνας από το αρχείο.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Αλλάξτε το μέγεθος της εικόνας σύμφωνα με τις ανάγκες σας (προαιρετικό).
                              Width = 100,
                              Height = 100,

                              // Ορίστε τη θέση της εικόνας στη σελίδα (προαιρετικό).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Ορισμός στοίχισης εικόνας
                              Alignment = HorizontalAlignment.Right
                          };

// Προσθέστε την εικόνα στη σελίδα.
page.AppendChildLast(image);
```

Δείχνει πώς να προσθέσετε ένα αρχείο από μια ροή σε ένα έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Attachments();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης Outline
Outline outline = new Outline(doc);

// Αρχικοποίηση αντικειμένου κλάσης OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Εκκινήστε το αντικείμενο κλάσης AttachedFile και περάστε επίσης τη διαδρομή του εικονιδίου του
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Προσθήκη συνημμένου αρχείου
    outlineElem.AppendChildLast(attachedFile);
}

// Προσθήκη κόμβου στοιχείου περιγράμματος
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου περιγράμματος
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

Όταν οι μεγάλες σελίδες του OneNote αποθηκεύονται σε μορφή pdf, χωρίζονται σε σελίδες. Το παράδειγμα δείχνει πώς να διαμορφώσετε τη λογική διαχωρισμού των αντικειμένων που βρίσκονται στα διαλείμματα της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Ή
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
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

Δείχνει πώς να δημιουργήσετε ένα έγγραφο με σελίδα τίτλου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Aspose.Note.Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Προεπιλεγμένο στυλ για όλο το κείμενο του εγγράφου.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Ορισμός ιδιοτήτων τίτλου σελίδας
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Προσθήκη κόμβου σελίδας στο έγγραφο
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Δείχνει πώς να προσθέσετε μια εικόνα από τη ροή σε ένα έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Φορτώστε τη δεύτερη εικόνα χρησιμοποιώντας το όνομα, την επέκταση και τη ροή της εικόνας.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Ορισμός στοίχισης εικόνας
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Δείχνει πώς να προσθέσετε μια εικόνα από αρχείο σε έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Εκκίνηση αντικειμένου κλάσης Outline και ορισμός ιδιοτήτων μετατόπισης
Outline outline = new Outline(doc);

// Αρχικοποίηση αντικειμένου κλάσης OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Φόρτωση εικόνας από τη διαδρομή του αρχείου.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ορισμός στοίχισης εικόνας
                              Alignment = HorizontalAlignment.Right
                          };

// Προσθέστε εικόνα
outlineElem.AppendChildLast(image);

// Προσθήκη στοιχείων περιγράμματος
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου Outline
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

Δείχνει πώς να δημιουργήσετε ένα έγγραφο με ένα κείμενο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Page page = new Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης Outline
Outline outline = new Outline(doc);

// Αρχικοποίηση αντικειμένου κλάσης OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Εκκίνηση αντικειμένου κλάσης TextStyle και ορισμός ιδιοτήτων μορφοποίησης
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Αρχικοποίηση αντικειμένου κλάσης RichText και εφαρμογή στυλ κειμένου
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Προσθήκη κόμβου εμπλουτισμένου κειμένου
outlineElem.AppendChildLast(text);

// Προσθήκη κόμβου OutlineElement
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου Outline
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε διαφορετικές μορφές.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Εκκίνηση του νέου εγγράφου
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Εκκίνηση της νέας σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Προεπιλεγμένο στυλ για όλο το κείμενο του εγγράφου.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθηκεύστε το έγγραφο του OneNote σε διαφορετικές μορφές, ορίστε το μέγεθος γραμματοσειράς κειμένου και εντοπίστε τις αλλαγές διάταξης με μη αυτόματο τρόπο.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
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

Δείχνει πώς να συνδέσετε μια υπερ-σύνδεση σε ένα κείμενο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tasks();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Προσθήκη στοιχείων περιγράμματος
outline.AppendChildLast(outlineElem);

// Αρχικοποίηση αντικειμένου κλάσης τίτλου
Title title = new Title() { TitleText = titleText };

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Page page = new Note.Page() { Title = title };

// Προσθήκη κόμβου Outline
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

Δείχνει τον τρόπο πρόσβασης στο περιεχόμενο ενός εγγράφου χρησιμοποιώντας τον επισκέπτη.

```csharp
public static void Run()
{
    // Η διαδρομή προς τον κατάλογο εγγράφων.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // Ανοίξτε το έγγραφο που θέλουμε να μετατρέψουμε.
    Document doc = new Document(dataDir + "Aspose.one");

    // Δημιουργήστε ένα αντικείμενο που κληρονομεί από την κλάση DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // Αυτό είναι το γνωστό μοτίβο επισκεπτών. Πάρτε το μοντέλο για να δεχτεί έναν επισκέπτη.
    // Το μοντέλο θα επαναληφθεί μέσω του εαυτού του καλώντας τις αντίστοιχες μεθόδους
    // στο αντικείμενο επισκέπτη (αυτό ονομάζεται επίσκεψη).
    //
    // Σημειώστε ότι κάθε κόμβος στο μοντέλο αντικειμένου έχει τη μέθοδο Accept και έτσι την επίσκεψη
    // μπορεί να εκτελεστεί όχι μόνο για ολόκληρο το έγγραφο, αλλά για οποιονδήποτε κόμβο του εγγράφου.
    doc.Accept(myConverter);

    // Μόλις ολοκληρωθεί η επίσκεψη, μπορούμε να ανακτήσουμε το αποτέλεσμα της λειτουργίας,
    // που σε αυτό το παράδειγμα, έχει συσσωρευτεί στον επισκέπτη.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// Απλή υλοποίηση της αποθήκευσης ενός εγγράφου σε μορφή απλού κειμένου. Υλοποιήθηκε ως Επισκέπτης.
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// Λαμβάνει το απλό κείμενο του εγγράφου που συγκεντρώθηκε από τον επισκέπτη.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// Προσθέτει κείμενο στην τρέχουσα έξοδο. Τιμά τη σημαία ενεργοποίησης/απενεργοποίησης εξόδου.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// Καλείται όταν εμφανίζεται ένας κόμβος εμπλουτισμένου κειμένου στο έγγραφο.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// Καλείται όταν συναντάται ένας κόμβος εγγράφου στο έγγραφο.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν εμφανίζεται ένας κόμβος σελίδας στο έγγραφο.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// Καλείται όταν ολοκληρωθεί η επεξεργασία ενός κόμβου Σελίδας.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// Καλείται όταν βρεθεί ένας κόμβος τίτλου στο έγγραφο.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν εμφανίζεται ένας κόμβος εικόνας στο έγγραφο.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν ένας κόμβος OutlineGroup συναντάται στο έγγραφο.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν συναντάται ένας κόμβος Outline στο έγγραφο.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// Καλείται όταν εμφανίζεται ένας κόμβος OutlineElement στο έγγραφο.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// Λαμβάνει τον συνολικό αριθμό των κόμβων από τον Επισκέπτη
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### Δείτε επίσης

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Page](../page/)
* interface [INotebookChildNode](../inotebookchildnode/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


