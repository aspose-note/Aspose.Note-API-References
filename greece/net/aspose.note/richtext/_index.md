---
title: Class RichText
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.RichText τάξη. Αντιπροσωπεύει ένα πλούσιο κείμενο.
type: docs
weight: 530
url: /el/net/aspose.note/richtext/
---
## RichText class

Αντιπροσωπεύει ένα πλούσιο κείμενο.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [RichText](richtext/#constructor)() | Αρχικοποιεί μια νέα παρουσία του`RichText` τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | Λαμβάνει ή ορίζει τη στοίχιση. |
| [Document](../../aspose.note/node/document/) { get; } | Λαμβάνει το έγγραφο του κόμβου. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτός ο κόμβος είναι σύνθετος. Εάν είναι αληθές, ο κόμβος μπορεί να έχει θυγατρικούς κόμβους. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [Length](../../aspose.note/richtext/length/) { get; } | Παίρνει το μήκος του κειμένου. |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | Λαμβάνει ή ορίζει το διάστιχο. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Λαμβάνει τον επόμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Παίρνει τον τύπο κόμβου. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | Λαμβάνει ή ορίζει το στυλ παραγράφου. Αυτές οι ρυθμίσεις χρησιμοποιούνται εάν δεν υπάρχει αντίστοιχο αντικείμενο TextStyle στοStyles συλλογή είτε αυτό το αντικείμενο δεν καθορίζει μια απαραίτητη ρύθμιση. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Λαμβάνει τον γονικό κόμβο. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Λαμβάνει τον προηγούμενο κόμβο στο ίδιο επίπεδο δέντρου κόμβου. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | Λαμβάνει ή ορίζει το ελάχιστο διάστημα μετά. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | Λαμβάνει ή ορίζει το ελάχιστο διάστημα πριν. |
| [Tags](../../aspose.note/richtext/tags/) { get; } | Λαμβάνει τη λίστα με όλες τις ετικέτες μιας παραγράφου. |
| [Text](../../aspose.note/richtext/text/) { get; set; } | Λαμβάνει ή ορίζει το κείμενο. Η συμβολοσειρά ΔΕΝ ΠΡΕΠΕΙ να περιέχει χαρακτήρες της τιμής 10 (τροφοδοσία γραμμής). |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | Λαμβάνει τη συλλογή των εκτελέσεων κειμένου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | Αποδέχεται τον επισκέπτη του κόμβου. |
| [Append](../../aspose.note/richtext/append/#append)(string) | Προσθέτει μια συμβολοσειρά στο τελευταίο εύρος κειμένου. |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | Προσθέτει μια συμβολοσειρά στο τέλος. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | Προσθέτει μια συμβολοσειρά στο μπροστινό μέρος του πρώτου εύρους κειμένου. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | Προσθέτει μια συμβολοσειρά στο μπροστινό μέρος. |
| [Clear](../../aspose.note/richtext/clear/)() | Διαγράφει το περιεχόμενο αυτής της παρουσίας. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | Επιστρέφει έναν απαριθμητή που επαναλαμβάνεται μέσω χαρακτήρων αυτού του αντικειμένου RichText. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | Επιστρέφει το μηδενικό ευρετήριο της πρώτης εμφάνισης του καθορισμένου χαρακτήρα Unicode σε αυτήν τη συμβολοσειρά. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | Επιστρέφει το μηδενικό ευρετήριο της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς σε αυτήν την εμφάνιση. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | Επιστρέφει το μηδενικό ευρετήριο της πρώτης εμφάνισης του καθορισμένου χαρακτήρα Unicode σε αυτήν τη συμβολοσειρά. Η αναζήτηση ξεκινά σε μια καθορισμένη θέση χαρακτήρων. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | Επιστρέφει το μηδενικό ευρετήριο της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς σε αυτήν την εμφάνιση. Η αναζήτηση ξεκινά σε μια καθορισμένη θέση χαρακτήρων. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | Επιστρέφει το μηδενικό ευρετήριο της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία. Μια παράμετρος καθορίζει τον τύπο αναζήτησης που θα χρησιμοποιηθεί για την καθορισμένη συμβολοσειρά. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | Επιστρέφει το μηδενικό ευρετήριο της πρώτης εμφάνισης του καθορισμένου χαρακτήρα σε αυτήν την εμφάνιση. Η αναζήτηση ξεκινά από μια καθορισμένη θέση χαρακτήρων και εξετάζει έναν καθορισμένο αριθμό θέσεων χαρακτήρων. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | Επιστρέφει το μηδενικό ευρετήριο της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς σε αυτήν την εμφάνιση. Η αναζήτηση ξεκινά από μια καθορισμένη θέση χαρακτήρων και εξετάζει έναν καθορισμένο αριθμό θέσεων χαρακτήρων. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | Επιστρέφει το μηδενικό ευρετήριο της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία. Οι παράμετροι καθορίζουν τη θέση έναρξης αναζήτησης στην τρέχουσα συμβολοσειρά και τον τύπο αναζήτησης που θα χρησιμοποιηθεί για την καθορισμένη συμβολοσειρά. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | Επιστρέφει το μηδενικό ευρετήριο της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία. |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | Εισάγει μια καθορισμένη συμβολοσειρά σε μια καθορισμένη θέση ευρετηρίου σε αυτήν την εμφάνιση. |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | Εισάγει μια καθορισμένη συμβολοσειρά με καθορισμένο στυλ σε μια καθορισμένη θέση ευρετηρίου σε αυτήν την εμφάνιση. |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | Καταργεί όλους τους χαρακτήρες στην τρέχουσα παρουσία, ξεκινώντας από μια καθορισμένη θέση και συνεχίζοντας μέχρι την τελευταία θέση. |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | Αφαιρεί καθορισμένο αριθμό χαρακτήρων στην τρέχουσα παρουσία που ξεκινά από μια καθορισμένη θέση. |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | Αντικαθιστά όλες τις εμφανίσεις ενός καθορισμένου χαρακτήρα Unicode σε αυτήν την περίπτωση με έναν άλλο καθορισμένο χαρακτήρα Unicode. |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία με μια άλλη καθορισμένη συμβολοσειρά. |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία με μια άλλη καθορισμένη συμβολοσειρά σε καθορισμένο στυλ. |
| [Trim](../../aspose.note/richtext/trim/#trim)() | Αφαιρεί όλους τους κύριους και τους επόμενους χαρακτήρες λευκού διαστήματος. |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | Καταργεί όλες τις κύριες και τις τελευταίες εμφανίσεις ενός χαρακτήρα. |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | Καταργεί όλες τις εμφανίσεις προπορευόμενου και τελικού ενός συνόλου χαρακτήρων που καθορίζονται σε έναν πίνακα. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | Καταργεί όλους τους χαρακτήρες κενού διαστήματος. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | Καταργεί όλα τα τελικά συμβάντα ενός χαρακτήρα. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | Καταργεί όλα τα τελικά συμβάντα ενός συνόλου χαρακτήρων που καθορίζονται σε έναν πίνακα. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | Αφαιρεί όλους τους κύριους χαρακτήρες λευκού διαστήματος. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | Καταργεί όλες τις κύριες εμφανίσεις ενός καθορισμένου χαρακτήρα. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | Καταργεί όλες τις κύριες εμφανίσεις ενός συνόλου χαρακτήρων που καθορίζονται σε έναν πίνακα. |

### Παραδείγματα

Δείχνει πώς να λαμβάνετε όλο το κείμενο από το έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ανάκτηση κειμένου
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Εκτύπωση κειμένου στην οθόνη εξόδου
Console.WriteLine(text);
```

Δείχνει πώς να λαμβάνετε όλο το κείμενο από τη σελίδα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη λίστας κόμβων σελίδας
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Ανάκτηση κειμένου
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Εκτύπωση κειμένου στην οθόνη εξόδου
    Console.WriteLine(text);
}
```

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

Δείχνει πώς να λαμβάνετε κείμενο από κάθε σειρά πίνακα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tables();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Λάβετε μια λίστα με κόμβους πίνακα
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Επανάληψη σε γραμμές πίνακα
    foreach (TableRow row in table)
    {
        // Ανάκτηση κειμένου
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Εκτύπωση κειμένου στην οθόνη εξόδου
        Console.WriteLine(text);
    }
}
```

Δείχνει πώς να λαμβάνετε κείμενο από έναν πίνακα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tables();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Λάβετε μια λίστα με κόμβους πίνακα
IList<Table> nodes = document.GetChildNodes<Table>();

// Ορισμός αριθμού τραπεζιών
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Ανάκτηση κειμένου
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Εκτύπωση κειμένου στην οθόνη εξόδου
    Console.WriteLine(text);
}
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

Δείχνει πώς να λαμβάνετε κείμενο από τα κελιά ενός πίνακα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tables();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Λάβετε μια λίστα με κόμβους πίνακα
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Επανάληψη σε γραμμές πίνακα
    foreach (TableRow row in table)
    {
        // Λήψη λίστας κόμβων TableCell
        // Επανάληψη μέσω των κελιών πίνακα
        foreach (TableCell cell in row)
        {
            // Ανάκτηση κειμένου
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Εκτύπωση κειμένου στην οθόνη εξόδου
            Console.WriteLine(text);
        }
    }
}
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

Δείχνει πώς να προσθέσετε νέα παράγραφο με ετικέτα.

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
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// Προσθήκη κόμβου κειμένου
outlineElem.AppendChildLast(text);

// Προσθήκη κόμβου στοιχείου περιγράμματος
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου περιγράμματος
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "AddTextNodeWithTag_out.one";
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

Δείχνει τον τρόπο πρόσβασης σε λεπτομέρειες μιας ετικέτας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Λήψη όλων των κόμβων RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Επανάληψη σε κάθε κόμβο
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Ανάκτηση ιδιοτήτων
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
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

Δείχνει πώς να προετοιμάσετε ένα πρότυπο για εβδομαδιαία συνάντηση.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
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

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


