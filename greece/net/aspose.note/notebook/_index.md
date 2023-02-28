---
title: Class Notebook
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Notebook τάξη. Αντιπροσωπεύει ένα σημειωματάριο Aspose.Note.
type: docs
weight: 410
url: /el/net/aspose.note/notebook/
---
## Notebook class

Αντιπροσωπεύει ένα σημειωματάριο Aspose.Note.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [Notebook](notebook/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`Notebook` τάξη. |
| [Notebook](notebook/#constructor_1)(Stream) | Αρχικοποιεί μια νέα παρουσία του`Notebook` class. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από μια ροή. |
| [Notebook](notebook/#constructor_3)(string) | Αρχικοποιεί μια νέα παρουσία του`Notebook` class. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από ένα αρχείο. |
| [Notebook](notebook/#constructor_2)(Stream, NotebookLoadOptions) | Αρχικοποιεί μια νέα παρουσία του`Notebook` class. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από μια ροή. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης. |
| [Notebook](notebook/#constructor_4)(string, NotebookLoadOptions) | Αρχικοποιεί μια νέα παρουσία του`Notebook` class. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από ένα αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών, όπως μια στρατηγική φόρτωσης για παιδιά ("τεμπέλης"/άμεση). |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Color](../../aspose.note/notebook/color/) { get; set; } | Παίρνει ή ρυθμίζει το χρώμα. |
| [Count](../../aspose.note/notebook/count/) { get; } | Παίρνει τον αριθμό των στοιχείων που περιέχονται στο`Notebook` . |
| [DisplayName](../../aspose.note/notebook/displayname/) { get; set; } | Λαμβάνει ή ορίζει το εμφανιζόμενο όνομα. |
| [FileFormat](../../aspose.note/notebook/fileformat/) { get; } | Λαμβάνει μορφή αρχείου (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid/) { get; } | Λαμβάνει το παγκοσμίως μοναδικό αναγνωριστικό του αντικειμένου. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το ιστορικό είναι ενεργοποιημένο. |
| [Item](../../aspose.note/notebook/item/) { get; } | Λαμβάνει τον θυγατρικό κόμβο σημειωματάριου με βάση το δεδομένο ευρετήριο. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild/)(INotebookChildNode) | Προσθέτει τον κόμβο στο τέλος της λίστας. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes/)() | Λήψη όλων των θυγατρικών κόμβων ανά τύπο κόμβου. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator/)() | Επιστρέφει έναν απαριθμητή που επαναλαμβάνεται μέσω θυγατρικών κόμβων του`Notebook` . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument)(Stream) | Προσθέτει έναν θυγατρικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο του OneNote από μια ροή. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_2)(string) | Προσθέτει έναν θυγατρικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο του OneNote από ένα αρχείο. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_1)(Stream, LoadOptions) | Προσθέτει έναν θυγατρικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο του OneNote από μια ροή. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_3)(string, LoadOptions) | Προσθέτει έναν θυγατρικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο του OneNote από ένα αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook)(Stream) | Προσθέτει έναν θυγατρικό κόμβο σημειωματάριου. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από μια ροή. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_2)(string) | Προσθέτει έναν θυγατρικό κόμβο σημειωματάριου. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από ένα αρχείο. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Προσθέτει έναν θυγατρικό κόμβο σημειωματάριου. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από μια ροή. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_3)(string, NotebookLoadOptions) | Προσθέτει έναν θυγατρικό κόμβο σημειωματάριου. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από ένα αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης. |
| [RemoveChild](../../aspose.note/notebook/removechild/)(INotebookChildNode) | Αφαιρεί τον θυγατρικό κόμβο. |
| [Save](../../aspose.note/notebook/save/#save)(Stream) | Αποθηκεύει το έγγραφο του OneNote σε μια ροή. |
| [Save](../../aspose.note/notebook/save/#save_3)(string) | Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο. |
| [Save](../../aspose.note/notebook/save/#save_2)(Stream, NotebookSaveOptions) | Αποθηκεύει το έγγραφο του OneNote σε μια ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [Save](../../aspose.note/notebook/save/#save_1)(Stream, SaveFormat) | Αποθηκεύει το έγγραφο του OneNote σε μια ροή με την καθορισμένη μορφή. |
| [Save](../../aspose.note/notebook/save/#save_5)(string, NotebookSaveOptions) | Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [Save](../../aspose.note/notebook/save/#save_4)(string, SaveFormat) | Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο στην καθορισμένη μορφή. |

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το σημειωματάριο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir);
```

Δείχνει πώς να αποθηκεύσετε σημειωματάριο σε μορφή pdf.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir);
```

Δείχνει πώς να αποθηκεύσετε το σημειωματάριο ως εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir);
```

Δείχνει πώς να λαμβάνετε όλο το κείμενο από ένα σημειωματάριο.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

Δείχνει πώς μπορείτε να αποθηκεύσετε πεπλατυσμένο σημειωματάριο σε μορφή pdf.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Αποθηκεύστε το Σημειωματάριο
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Δείχνει πώς να επαναλαμβάνετε τα έγγραφα ενός σημειωματάριου φορτώνοντάς τα νωχελικά.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// Από προεπιλογή η φόρτωση των παιδιών είναι "τεμπέλης".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Η πραγματική φόρτωση του θυγατρικού εγγράφου πραγματοποιείται μόνο εδώ.
    // Κάντε κάτι με το θυγατρικό έγγραφο
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

Δείχνει πώς να φορτώσετε το σημειωματάριο από μια ροή.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
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

Δείχνει πώς να αφαιρέσετε μια ενότητα από ένα σημειωματάριο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Διασχίστε τους θυγατρικούς κόμβους του για αναζήτηση του επιθυμητού θυγατρικού στοιχείου
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Αφαιρέστε το Θυγατρικό Στοιχείο από το Σημειωματάριο
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir);
```

Δείχνει τον τρόπο επανάληψης μέσω προφορτωμένων εγγράφων ενός σημειωματάριου.

```csharp
// Από προεπιλογή η φόρτωση των παιδιών είναι "τεμπέλης".
// Επομένως, για την άμεση φόρτωση πραγματοποιήθηκε,
// είναι απαραίτητο να ορίσετε τη σημαία NotebookLoadOptions.InstantLoading.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Όλα τα θυγατρικά έγγραφα έχουν ήδη φορτωθεί.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Κάντε κάτι με το θυγατρικό έγγραφο
}
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

### Δείτε επίσης

* interface [INotebookChildNode](../inotebookchildnode/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


