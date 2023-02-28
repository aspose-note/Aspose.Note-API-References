---
title: Class Page
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Page τάξη. Αντιπροσωπεύει μια σελίδα.
type: docs
weight: 480
url: /el/net/aspose.note/page/
---
## Page class

Αντιπροσωπεύει μια σελίδα.

```csharp
public sealed class Page : CompositeNode<IPageChildNode>
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [Page](page/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`Page` τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Author](../../aspose.note/page/author/) { get; set; } | Λαμβάνει ή ορίζει τον συγγραφέα. |
| [BackgroundColor](../../aspose.note/page/backgroundcolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα φόντου της σελίδας. |
| [CreationTime](../../aspose.note/page/creationtime/) { get; set; } | Λαμβάνει ή ρυθμίζει το χρόνο δημιουργίας. |
| [Document](../../aspose.note/node/document/) { get; } | Λαμβάνει το έγγραφο του κόμβου. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [IsConflictPage](../../aspose.note/page/isconflictpage/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν αυτή η σελίδα είναι σελίδα διένεξης. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/page/lastmodifiedtime/) { get; set; } | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [Level](../../aspose.note/page/level/) { get; set; } | Παίρνει ή ρυθμίζει το επίπεδο. |
| [Margin](../../aspose.note/page/margin/) { get; set; } | Λαμβάνει ή ορίζει το περιθώριο. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Λαμβάνει τον επόμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Παίρνει τον τύπο κόμβου. |
| [PageContentRevisionSummary](../../aspose.note/page/pagecontentrevisionsummary/) { get; set; } | Λαμβάνει ή ορίζει τη σύνοψη αναθεώρησης για τη σελίδα και τους θυγατρικούς κόμβους. |
| [PageLayoutSize](../../aspose.note/page/pagelayoutsize/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος διάταξης της σελίδας που εμφανίζεται στο πρόγραμμα επεξεργασίας. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Λαμβάνει τον γονικό κόμβο. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Λαμβάνει τον προηγούμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [SizeType](../../aspose.note/page/sizetype/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο μεγέθους μιας σελίδας. |
| [Title](../../aspose.note/page/title/) { get; set; } | Παίρνει ή ορίζει τον τίτλο. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [Accept](../../aspose.note/page/accept/)(DocumentVisitor) | Αποδέχεται τον επισκέπτη του κόμβου. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [Clone](../../aspose.note/page/clone/)(bool) | Κλωνοποιεί τη σελίδα. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/page/getchildnodes/#getchildnodes_1)() | Λήψη όλων των θυγατρικών κόμβων της σελίδας ανά τύπο κόμβου. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IPageChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IPageChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Παραδείγματα

Δείχνει πώς να ορίσετε το χρώμα φόντου της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
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

Δείχνει πώς να ορίσετε έναν τίτλο για μια σελίδα.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
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

Δείχνει πώς να επεξεργαστείτε τις μετα-πληροφορίες της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Ανάγνωση περίληψης αναθεώρησης περιεχομένου για αυτήν τη σελίδα
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Ενημέρωση περίληψης αναθεώρησης σελίδας για αυτήν τη σελίδα
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

Δείχνει πώς να περάσετε από όλες τις σελίδες και να κάνετε μια αντικατάσταση στο κείμενο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη όλων των κόμβων RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Αντικατάσταση κειμένου σχήματος
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Αποθήκευση σε οποιαδήποτε υποστηριζόμενη μορφή αρχείου
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Δείχνει πώς να περάσετε μέσα από το κείμενο της σελίδας και να κάνετε μια αντικατάσταση.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Λήψη όλων των κόμβων RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Αντικατάσταση κειμένου σχήματος
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Αποθήκευση σε οποιαδήποτε υποστηριζόμενη μορφή αρχείου
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
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

Δείχνει πώς να προσθέσετε νέα εικόνα με ετικέτα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης Outline
Outline outline = new Outline(doc);

// Αρχικοποίηση αντικειμένου κλάσης OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Φόρτωση εικόνας
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Εισαγωγή εικόνας στον κόμβο του εγγράφου
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Προσθήκη κόμβου στοιχείου περιγράμματος
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου περιγράμματος
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
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

Δείχνει τον τρόπο εισαγωγής νέας λίστας με κινεζική αρίθμηση.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Εκκίνηση εγγράφου OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// Αρχικοποίηση σελίδας OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Εφαρμογή ρυθμίσεων στυλ κειμένου
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Οι αριθμοί στο ίδιο περίγραμμα προσαυξάνονται αυτόματα.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//---------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//---------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//---------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Δείχνει τον τρόπο εισαγωγής νέας λίστας με κουκκίδες.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης Outline
Outline outline = new Outline(doc);

// Εκκίνηση αντικειμένου κλάσης TextStyle και ορισμός ιδιοτήτων μορφοποίησης
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Εκκίνηση αντικειμένων κλάσης OutlineElement και εφαρμογή κουκκίδων
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Αρχικοποίηση αντικειμένου κλάσης RichText και εφαρμογή στυλ κειμένου
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Προσθήκη στοιχείων περιγράμματος
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Προσθήκη κόμβου Outline
page.AppendChildLast(outline);
// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Δείχνει τον τρόπο εισαγωγής νέας λίστας με αρίθμηση.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης Outline
Outline outline = new Outline(doc);

// Εκκίνηση αντικειμένου κλάσης TextStyle και ορισμός ιδιοτήτων μορφοποίησης
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Αρχικοποίηση αντικειμένων κλάσης OutlineElement και εφαρμογή αρίθμησης
// Οι αριθμοί στο ίδιο περίγραμμα προσαυξάνονται αυτόματα.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Προσθήκη στοιχείων περιγράμματος
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Προσθήκη κόμβου Outline
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

Δείχνει πώς να προσθέσετε μια σελίδα με μια υποσελίδα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας και ορισμός του επιπέδου του
Aspose.Note.Page page1 = new Aspose.Note.Page(doc) { Level = 1 };

// Αρχικοποίηση αντικειμένου κλάσης σελίδας και ορισμός του επιπέδου του
Aspose.Note.Page page2 = new Aspose.Note.Page(doc) { Level = 2 };

// Αρχικοποίηση αντικειμένου κλάσης σελίδας και ορισμός του επιπέδου του
Aspose.Note.Page page3 = new Aspose.Note.Page(doc) { Level = 1 };

/*---------- Adding nodes to first Page ----------*/
Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "First page.", ParagraphStyle = textStyle };
outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page1.AppendChildLast(outline);

/*---------- Adding nodes to second Page ----------*/
var outline2 = new Outline(doc);
var outlineElem2 = new OutlineElement(doc);
var textStyle2 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text2 = new RichText(doc) { Text = "Second page.", ParagraphStyle = textStyle2 };
outlineElem2.AppendChildLast(text2);
outline2.AppendChildLast(outlineElem2);
page2.AppendChildLast(outline2);

/*---------- Adding nodes to third Page ----------*/
var outline3 = new Outline(doc);
var outlineElem3 = new OutlineElement(doc);
var textStyle3 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text3 = new RichText(doc) { Text = "Third page.", ParagraphStyle = textStyle3 };
outlineElem3.AppendChildLast(text3);
outline3.AppendChildLast(outlineElem3);
page3.AppendChildLast(outline3);

/*---------- Add pages to the OneNote Document ----------*/
doc.AppendChildLast(page1);
doc.AppendChildLast(page2);
doc.AppendChildLast(page3);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "CreateDocWithRootAndSubPages_out.one";
doc.Save(dataDir);
```

### Δείτε επίσης

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IPageChildNode](../ipagechildnode/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


