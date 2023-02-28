---
title: Style.FontColor
second_title: Aspose.Note for .NET API Reference
description: Style ιδιοκτησία. Παίρνει ή ορίζει το χρώμα της γραμματοσειράς.
type: docs
weight: 10
url: /el/net/aspose.note/style/fontcolor/
---
## Style.FontColor property

Παίρνει ή ορίζει το χρώμα της γραμματοσειράς.

```csharp
public Color FontColor { get; set; }
```

### Παραδείγματα

Δείχνει πώς να αλλάξετε στυλ για ένα κείμενο.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Αποκτήστε έναν συγκεκριμένο κόμβο εμπλουτισμένου κειμένου
RichText richText = document.GetChildNodes<RichText>().First();

foreach (var run in richText.TextRuns)
{
    // Ορισμός χρώματος γραμματοσειράς
    run.Style.FontColor = Color.Yellow;

    // Ορισμός χρώματος επισήμανσης
    run.Style.Highlight = Color.Blue;

    // Ορισμός μεγέθους γραμματοσειράς
    run.Style.FontSize = 20;
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

Δείχνει πώς να συνθέσετε έναν πίνακα με κείμενο με διάφορα στυλ.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var headerText = new RichText() { ParagraphStyle = new ParagraphStyle() { FontSize = 18, IsBold = true }, Alignment = HorizontalAlignment.Center }
                    .Append("Super contest for suppliers.");

var page = new Page();
var outline = page.AppendChildLast(new Outline() { HorizontalOffset = 50 });
outline.AppendChildLast(new OutlineElement()).AppendChildLast(headerText);

// Περίληψη κειμένου πριν από τον πίνακα
var bodyTextHeader = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
bodyTextHeader.Append("This is the final ranking of proposals got from our suppliers.");

var ranking = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new Table());
var headerRow = ranking.AppendChildFirst(new TableRow());

var headerStyle = ParagraphStyle.Default;
headerStyle.IsBold = true;

// Ας προσθέσουμε ένα σύνολο στηλών και μια γραμμή κεφαλίδας
var backGroundColor = Color.LightGray;
foreach (var header in new[] { "Supplier", "Contacts", "Score A", "Score B", "Score C", "Final score", "Attached materials", "Comments" })
{
    ranking.Columns.Add(new TableColumn());
    headerRow.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
             .AppendChildLast(new OutlineElement())
             .AppendChildLast(new RichText() { ParagraphStyle = headerStyle })
                .Append(header);
}

// Ας κάνουμε 5 κενές σειρές. Οι σειρές έχουν εναλλάξ χρώμα φόντου
for (int i = 0; i < 5; i++)
{
    backGroundColor = backGroundColor.IsEmpty ? Color.LightGray : Color.Empty;

    var row = ranking.AppendChildLast(new TableRow());
    for (int j = 0; j < ranking.Columns.Count(); j++)
    {
        row.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
           .AppendChildLast(new OutlineElement())
           .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
    }
}

// Ας προσθέσουμε κάποιο πρότυπο για περιεχόμενο στη στήλη "Επαφές".
foreach (var row in ranking.Skip(1))
{
    var contactsCell = row.ElementAt(1);
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("Web: ").Append("link", new TextStyle() { HyperlinkAddress = "www.link.com", IsHyperlink = true });
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("E-mail: ").Append("mail", new TextStyle() { HyperlinkAddress = "mailto:hi@link.com", IsHyperlink = true });
}

var d = new Document();
d.AppendChildLast(page);
d.Save(Path.Combine(dataDir, "ComposeTable_out.one"));
```

### Δείτε επίσης

* class [Style](../)
* χώρος ονομάτων [Aspose.Note](../../style/)
* συνέλευση [Aspose.Note](../../../)


