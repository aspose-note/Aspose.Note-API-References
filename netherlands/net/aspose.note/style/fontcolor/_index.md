---
title: Style.FontColor
second_title: Aspose.Note voor .NET API-referentie
description: Style eigendom. Hiermee wordt de letterkleur opgehaald of ingesteld.
type: docs
weight: 10
url: /nl/net/aspose.note/style/fontcolor/
---
## Style.FontColor property

Hiermee wordt de letterkleur opgehaald of ingesteld.

```csharp
public Color FontColor { get; set; }
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

Laat zien hoe u de donkere themastijl toepast op een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
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

Laat zien hoe u een nieuwe lijst met Chinese nummering invoegt.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Initialiseer OneNote-document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initialiseer de OneNote-pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Tekststijlinstellingen toepassen
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Getallen in dezelfde opbouw worden automatisch opgehoogd.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//---------------------------------------------------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//---------------------------------------------------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//---------------------------------------------------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Laat zien hoe je een nieuwe lijst met opsommingstekens invoegt.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Maak een object van de klasse Document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject TextStyle en stel opmaakeigenschappen in
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialiseer de klasse-objecten van OutlineElement en pas opsommingstekens toe
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Initialiseer het RichText-klasseobject en pas tekststijl toe
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);
// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Laat zien hoe u een nieuwe lijst met nummering invoegt.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject TextStyle en stel opmaakeigenschappen in
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialiseer de klasse-objecten van OutlineElement en pas nummering toe
// Getallen in dezelfde opbouw worden automatisch opgehoogd.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

Laat zien hoe u een hyperlink aan een tekst koppelt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tasks();

// Maak een object van de klasse Document
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

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem);

// Initialiseer het titelklasse-object
Title title = new Title() { TitleText = titleText };

// Initialiseer het paginaklasse-object
Page page = new Note.Page() { Title = title };

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
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


