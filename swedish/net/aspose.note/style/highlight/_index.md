---
title: Style.Highlight
second_title: Aspose.Note för .NET API-referens
description: Style fast egendom. Hämtar eller ställer in högdagerfärgen.
type: docs
weight: 50
url: /sv/net/aspose.note/style/highlight/
---
## Style.Highlight property

Hämtar eller ställer in högdagerfärgen.

```csharp
public Color Highlight { get; set; }
```

### Exempel

Visar hur man ändrar stil för en text.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Hämta en viss RichText-nod
RichText richText = document.GetChildNodes<RichText>().First();

foreach (var run in richText.TextRuns)
{
    // Ställ in teckensnittsfärg
    run.Style.FontColor = Color.Yellow;

    // Ställ in högdagerfärg
    run.Style.Highlight = Color.Blue;

    // Ställ in teckenstorlek
    run.Style.FontSize = 20;
}
```

Visar hur man komponerar en tabell med text med olika stilar.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var headerText = new RichText() { ParagraphStyle = new ParagraphStyle() { FontSize = 18, IsBold = true }, Alignment = HorizontalAlignment.Center }
                    .Append("Super contest for suppliers.");

var page = new Page();
var outline = page.AppendChildLast(new Outline() { HorizontalOffset = 50 });
outline.AppendChildLast(new OutlineElement()).AppendChildLast(headerText);

// Sammanfattningstext före tabell
var bodyTextHeader = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
bodyTextHeader.Append("This is the final ranking of proposals got from our suppliers.");

var ranking = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new Table());
var headerRow = ranking.AppendChildFirst(new TableRow());

var headerStyle = ParagraphStyle.Default;
headerStyle.IsBold = true;

// Låt oss lägga till en uppsättning kolumner och en rubrikrad
var backGroundColor = Color.LightGray;
foreach (var header in new[] { "Supplier", "Contacts", "Score A", "Score B", "Score C", "Final score", "Attached materials", "Comments" })
{
    ranking.Columns.Add(new TableColumn());
    headerRow.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
             .AppendChildLast(new OutlineElement())
             .AppendChildLast(new RichText() { ParagraphStyle = headerStyle })
                .Append(header);
}

// Låt oss 5 tomma rader. Rader har växlande bakgrundsfärg
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

// Låt oss lägga till en mall för innehåll i kolumnen "Kontakter".
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

### Se även

* class [Style](../)
* namnutrymme [Aspose.Note](../../style/)
* hopsättning [Aspose.Note](../../../)


