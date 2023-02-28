---
title: Class Image
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Image τάξη. Αντιπροσωπεύει μια εικόνα.
type: docs
weight: 250
url: /el/net/aspose.note/image/
---
## Image class

Αντιπροσωπεύει μια εικόνα.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [Image](image/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`Image` τάξη. |
| [Image](image/#constructor_4)(string, Stream) | Αρχικοποιεί μια νέα παρουσία του`Image` τάξη. |
| [Image](image/#constructor_5)(string, string, string) | Αρχικοποιεί μια νέα παρουσία του`Image` τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | Λαμβάνει ή ορίζει τη στοίχιση. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | Λαμβάνει ή ορίζει ένα σώμα εναλλακτικού κειμένου για την εικόνα. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | Λαμβάνει ή ορίζει έναν τίτλο εναλλακτικού κειμένου για την εικόνα. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | Λαμβάνει το χώρο αποθήκευσης δεδομένων εικόνας. |
| [Document](../../aspose.note/node/document/) { get; } | Λαμβάνει το έγγραφο του κόμβου. |
| [FileName](../../aspose.note/image/filename/) { get; } | Λαμβάνει το όνομα αρχείου. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | Λαμβάνει τη διαδρομή προς το αρχείο εικόνας. |
| [Format](../../aspose.note/image/format/) { get; } | Λαμβάνει τη μορφή της εικόνας. |
| [Height](../../aspose.note/image/height/) { get; set; } | Λαμβάνει ή ορίζει το ύψος. Αυτό είναι το πραγματικό ύψος της εικόνας στο έγγραφο MS OneNote. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | Λαμβάνει ή ορίζει την οριζόντια μετατόπιση. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | Λαμβάνει ή ορίζει την υπερ-σύνδεση που σχετίζεται με την εικόνα. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | Βρίσκει αν η εικόνα είναι εικόνα φόντου. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτός ο κόμβος είναι σύνθετος. Εάν είναι αληθές, ο κόμβος μπορεί να έχει θυγατρικούς κόμβους. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | Λαμβάνει ή ορίζει τον χρόνο τελευταίας τροποποίησης. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Λαμβάνει τον επόμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Παίρνει τον τύπο κόμβου. |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | Λαμβάνει το αρχικό ύψος. Αυτό είναι το αρχικό πλάτος της εικόνας, πριν από την αλλαγή μεγέθους. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | Λαμβάνει το αρχικό πλάτος. Αυτό είναι το αρχικό πλάτος της εικόνας, πριν από την αλλαγή μεγέθους. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Λαμβάνει τον γονικό κόμβο. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Λαμβάνει τον προηγούμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [Tags](../../aspose.note/image/tags/) { get; } | Λαμβάνει τη λίστα με όλες τις ετικέτες μιας παραγράφου. |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | Λαμβάνει ή ορίζει την κατακόρυφη μετατόπιση. |
| [Width](../../aspose.note/image/width/) { get; set; } | Λαμβάνει ή ορίζει το πλάτος. Αυτό είναι το πραγματικό πλάτος της εικόνας στο έγγραφο MS OneNote. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | Αποδέχεται τον επισκέπτη του κόμβου. |

### Παραδείγματα

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

### Δείτε επίσης

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


