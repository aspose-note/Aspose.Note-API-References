---
title: Style.Highlight
second_title: Aspose.Note for .NET API Reference
description: Style ιδιοκτησία. Λαμβάνει ή ορίζει το χρώμα επισήμανσης.
type: docs
weight: 50
url: /el/net/aspose.note/style/highlight/
---
## Style.Highlight property

Λαμβάνει ή ορίζει το χρώμα επισήμανσης.

```csharp
public Color Highlight { get; set; }
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


