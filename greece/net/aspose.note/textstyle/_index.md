---
title: Class TextStyle
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.TextStyle τάξη. Καθορίζει το στυλ κειμένου.
type: docs
weight: 970
url: /el/net/aspose.note/textstyle/
---
## TextStyle class

Καθορίζει το στυλ κειμένου.

```csharp
public sealed class TextStyle : Style
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [TextStyle](textstyle/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | Αποκτά το στυλ με την κουλτούρα "en-US". |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | Λαμβάνει προεπιλεγμένο στυλ για την ημερομηνία τίτλου στο MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | Λαμβάνει το προεπιλεγμένο στυλ για το κείμενο τίτλου στο MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | Αποκτά προεπιλεγμένο στυλ για την ώρα τίτλου στο MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Παίρνει ή ορίζει το χρώμα της γραμματοσειράς. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Λαμβάνει ή ορίζει το όνομα της γραμματοσειράς. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Λαμβάνει ή ορίζει το μέγεθος της γραμματοσειράς. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Παίρνει το στυλ γραμματοσειράς. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα επισήμανσης. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | Λαμβάνει ή ορίζει τη διεύθυνση υπερσύνδεσης. Πρέπει να οριστεί εάν η τιμή του[`IsHyperlink`](./ishyperlink/) Η ιδιότητα είναι αληθής. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ του κειμένου είναι έντονη. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι κρυφό. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι υπερσύνδεσμος. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι πλάγιο. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι μαθηματικής μορφοποίησης. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι διαγραμμένο. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι δείκτης. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι εκθέτης. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ κειμένου είναι υπογραμμισμένο. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | Λαμβάνει ή ορίζει τη γλώσσα του κειμένου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | Χρησιμεύει ως συνάρτηση κατακερματισμού για τον τύπο. |

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

Ορισμός γλώσσας διόρθωσης για ένα κείμενο.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
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

### Δείτε επίσης

* class [Style](../style/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


