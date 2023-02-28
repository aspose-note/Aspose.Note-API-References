---
title: Class ParagraphStyle
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.ParagraphStyle klas. Tekststijlinstellingen die moeten worden gebruikt als er geen overeenkomend TextStyleobject isStyles collectie of dit object specificeert geen benodigde instelling.
type: docs
weight: 510
url: /nl/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

Tekststijlinstellingen die moeten worden gebruikt als er geen overeenkomend TextStyle-object isStyles collectie of dit object specificeert geen benodigde instelling.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | Initialiseert een nieuw exemplaar van het`ParagraphStyle` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | Krijgt de ParagraphStyle met standaardinstellingen. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Hiermee wordt de letterkleur opgehaald of ingesteld. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Haalt de lettertypenaam op of stelt deze in. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Hiermee wordt de lettergrootte opgehaald of ingesteld. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Krijgt de lettertypestijl. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Haalt of stelt de markeringskleur in. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl vet is. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl cursief is. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl doorgestreept is. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl subscript is. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl superscript is. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl onderstreept is. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | Dient als hash-functie voor het type. |

### Voorbeelden

Laten we de titels van de pagina onder andere kopteksten benadrukken door de lettergrootte te vergroten.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Herhaal de paginatitels.
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

Laten we de wijzigingen in de laatste tekst benadrukken door te markeren.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Ontvang RichText-knooppunten die vorige week zijn gewijzigd.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Markeringskleur instellen
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Markeringskleur instellen
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Manipuleer op tekstformaat met behulp van alineastijl.

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

### Zie ook

* class [Style](../style/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


