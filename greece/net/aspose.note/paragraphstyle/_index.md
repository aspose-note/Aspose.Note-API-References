---
title: Class ParagraphStyle
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.ParagraphStyle τάξη. Ρυθμίσεις στυλ κειμένου που θα χρησιμοποιηθούν εάν δεν υπάρχει αντίστοιχο αντικείμενο TextStyleStyles συλλογή είτε αυτό το αντικείμενο δεν καθορίζει μια απαραίτητη ρύθμιση.
type: docs
weight: 510
url: /el/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

Ρυθμίσεις στυλ κειμένου που θα χρησιμοποιηθούν εάν δεν υπάρχει αντίστοιχο αντικείμενο TextStyleStyles συλλογή είτε αυτό το αντικείμενο δεν καθορίζει μια απαραίτητη ρύθμιση.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | Αρχικοποιεί μια νέα παρουσία του`ParagraphStyle` τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | Λαμβάνει το ParagraphStyle με προεπιλεγμένες ρυθμίσεις. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Παίρνει ή ορίζει το χρώμα της γραμματοσειράς. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Λαμβάνει ή ορίζει το όνομα της γραμματοσειράς. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος της γραμματοσειράς. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Παίρνει το στυλ γραμματοσειράς. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα επισήμανσης. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ του κειμένου είναι έντονη. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι πλάγιο. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι διαγραμμένο. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι δείκτης. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι εκθέτης. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι υπογραμμισμένο. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | Χρησιμεύει ως συνάρτηση κατακερματισμού για τον τύπο. |

### Παραδείγματα

Ας τονίσουμε τους τίτλους της σελίδας μεταξύ άλλων κεφαλίδων αυξάνοντας το μέγεθος της γραμματοσειράς.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Επανάληψη στους τίτλους της σελίδας.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

Ας τονίσουμε τις τελευταίες αλλαγές του κειμένου επισημαίνοντας.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Λάβετε κόμβους εμπλουτισμένου κειμένου που τροποποιήθηκαν την περασμένη εβδομάδα.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Ορισμός χρώματος επισήμανσης
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Ορισμός χρώματος επισήμανσης
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Χειριστείτε με μορφή κειμένου χρησιμοποιώντας στυλ παραγράφου.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
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

### Δείτε επίσης

* class [Style](../style/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


