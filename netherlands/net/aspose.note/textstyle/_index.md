---
title: Class TextStyle
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.TextStyle klas. Specificeert de tekststijl.
type: docs
weight: 970
url: /nl/net/aspose.note/textstyle/
---
## TextStyle class

Specificeert de tekststijl.

```csharp
public sealed class TextStyle : Style
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [TextStyle](textstyle/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | Past bij de "en-US"-cultuur. |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | Krijgt standaardstijl voor titeldatum in MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | Krijgt standaardstijl voor titeltekst in MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | Krijgt standaardstijl voor titeltijd in MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Hiermee wordt de letterkleur opgehaald of ingesteld. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Haalt de lettertypenaam op of stelt deze in. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Hiermee wordt de lettergrootte opgehaald of ingesteld. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Krijgt de lettertypestijl. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Haalt of stelt de markeringskleur in. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | Haalt of stelt het hyperlinkadres in. Moet worden ingesteld als de waarde van de[`IsHyperlink`](./ishyperlink/) eigenschap is waar. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl vet is. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | Haalt of stelt een waarde in die aangeeft of de tekststijl verborgen is. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl een hyperlink is. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl cursief is. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl wiskundige opmaak is. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl doorgestreept is. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl subscript is. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl superscript is. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl onderstreept is. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | Haalt de taal van de tekst op of stelt deze in. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | Dient als hash-functie voor het type. |

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

Taal voor proeflezen instellen voor een tekst.

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

### Zie ook

* class [Style](../style/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


