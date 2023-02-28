---
title: Class NumberList
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.NumberList τάξη. Αντιπροσωπεύει την αριθμημένη ή με κουκκίδες λίστα.
type: docs
weight: 440
url: /el/net/aspose.note/numberlist/
---
## NumberList class

Αντιπροσωπεύει την αριθμημένη ή με κουκκίδες λίστα.

```csharp
public class NumberList
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | Αρχικοποιεί μια νέα παρουσία του`NumberList`class. Αυτή η παρουσία αντιπροσωπεύει μια λίστα με κουκκίδες. |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | Αρχικοποιεί μια νέα παρουσία του`NumberList` class. Αυτή η παρουσία αντιπροσωπεύει μια αριθμημένη λίστα. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | Λαμβάνει ή ορίζει το όνομα της γραμματοσειράς. |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | Παίρνει ή ορίζει το χρώμα της γραμματοσειράς. |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος της γραμματοσειράς. |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | Λαμβάνει ή ορίζει τη μορφή της κεφαλίδας γραμμής. Για λίστες με κουκκίδες αντιπροσωπεύει ένα σύμβολο κουκκίδας. |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ του κειμένου είναι έντονη. |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι πλάγιο. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | Λαμβάνει ή ορίζει τη μορφή αριθμού που χρησιμοποιείται για μια ομάδα αυτόματα αριθμημένων αντικειμένων. Θα πρέπει να είναι null για λίστες με κουκκίδες. |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | Λαμβάνει ή ορίζει την αριθμητική τιμή που αντικαθιστά την τιμή του αυτόματου αριθμού του στοιχείου λίστας. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | Χρησιμεύει ως συνάρτηση κατακερματισμού για τον τύπο. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | Λαμβάνει την αριθμημένη κεφαλίδα λίστας. |

### Παραδείγματα

Δείχνει πώς να ανακτήσετε πληροφορίες σχετικά με τη μορφοποίηση της λίστας.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Ανακτήστε έναν κόμβο συλλογής του στοιχείου περιγράμματος
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Επανάληψη σε κάθε κόμβο
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Ανάκτηση ονόματος γραμματοσειράς
        Console.WriteLine("Font Name: " + list.Font);

        // Ανάκτηση μήκους γραμματοσειράς
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Ανάκτηση μεγέθους γραμματοσειράς
        Console.WriteLine("Font Size: " + list.FontSize);

        // Ανάκτηση χρώματος γραμματοσειράς
        Console.WriteLine("Font Color: " + list.FontColor);

        // Ανάκτηση μορφής
        Console.WriteLine("Font format: " + list.Format);

        // Επιλέξτε έντονη γραφή
        Console.WriteLine("Is bold: " + list.IsBold);

        // Έλεγχος πλάγιας γραφής
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
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

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


