---
title: Style.Highlight
second_title: Aspose.Note voor .NET API-referentie
description: Style eigendom. Haalt of stelt de markeringskleur in.
type: docs
weight: 50
url: /nl/net/aspose.note/style/highlight/
---
## Style.Highlight property

Haalt of stelt de markeringskleur in.

```csharp
public Color Highlight { get; set; }
```

### Voorbeelden

Laat zien hoe u de stijl van een tekst kunt wijzigen.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Haal een bepaald RichText-knooppunt op
RichText richText = document.GetChildNodes<RichText>().First();

foreach (var run in richText.TextRuns)
{
    // Letterkleur instellen
    run.Style.FontColor = Color.Yellow;

    // Markeringskleur instellen
    run.Style.Highlight = Color.Blue;

    // Lettergrootte instellen
    run.Style.FontSize = 20;
}
```

Laat zien hoe je een tabel samenstelt met tekst met verschillende stijlen.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var headerText = new RichText() { ParagraphStyle = new ParagraphStyle() { FontSize = 18, IsBold = true }, Alignment = HorizontalAlignment.Center }
                    .Append("Super contest for suppliers.");

var page = new Page();
var outline = page.AppendChildLast(new Outline() { HorizontalOffset = 50 });
outline.AppendChildLast(new OutlineElement()).AppendChildLast(headerText);

// Overzichtstekst voor tabel
var bodyTextHeader = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
bodyTextHeader.Append("This is the final ranking of proposals got from our suppliers.");

var ranking = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new Table());
var headerRow = ranking.AppendChildFirst(new TableRow());

var headerStyle = ParagraphStyle.Default;
headerStyle.IsBold = true;

// Laten we een set kolommen en een koprij toevoegen
var backGroundColor = Color.LightGray;
foreach (var header in new[] { "Supplier", "Contacts", "Score A", "Score B", "Score C", "Final score", "Attached materials", "Comments" })
{
    ranking.Columns.Add(new TableColumn());
    headerRow.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
             .AppendChildLast(new OutlineElement())
             .AppendChildLast(new RichText() { ParagraphStyle = headerStyle })
                .Append(header);
}

// Laten we 5 lege rijen maken. Rijen hebben een wisselende achtergrondkleur
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

// Laten we een sjabloon toevoegen voor inhoud in de kolom 'Contacten'
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

### Zie ook

* class [Style](../)
* naamruimte [Aspose.Note](../../style/)
* montage [Aspose.Note](../../../)


