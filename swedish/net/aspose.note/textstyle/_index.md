---
title: Class TextStyle
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.TextStyle klass. Anger textstilen.
type: docs
weight: 970
url: /sv/net/aspose.note/textstyle/
---
## TextStyle class

Anger textstilen.

```csharp
public sealed class TextStyle : Style
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [TextStyle](textstyle/)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | Får stilen med "en-US" kultur. |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | Får standardstil för titeldatum i MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | Får standardstil för titeltext i MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | Får standardstil för titeltid i MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Hämtar eller ställer in teckensnittsfärgen. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Hämtar eller ställer in teckensnittsnamnet. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Hämtar eller ställer in teckenstorleken. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Hämtar teckensnittsstilen. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Hämtar eller ställer in högdagerfärgen. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | Hämtar eller ställer in hyperlänkadressen. Måste ställas in om värdet på[`IsHyperlink`](./ishyperlink/) egenskapen är sann. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är fetstil. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är dold. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är hyperlänk. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är kursiv. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är matematisk formatering. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är genomstruken. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är nedsänkt. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är upphöjd. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är understruken. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | Hämtar eller ställer in språket för texten. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | Bestämmer om det angivna objektet är lika med det aktuella objektet. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | Bestämmer om det angivna objektet är lika med det aktuella objektet. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | Fungerar som en hashfunktion för typen. |

### Exempel

Låt oss betona sidans titlar bland andra rubriker genom att öka teckensnittets storlek.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Iterera genom sidans titlar.
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

Låt oss betona de senaste textens ändringar genom att markera.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Få RichText-noder modifierade förra veckan.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Ställ in högdagerfärg
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Ställ in högdagerfärg
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Ställ in korrekturspråk för en text.

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

Manipulera efter textformat med hjälp av styckeformat.

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

Visar hur man binder en hyperlänk till en text.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tasks();

// Skapa ett objekt av klassen Document
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

// Lägg till konturelement
outline.AppendChildLast(outlineElem);

// Initiera Title-klassobjekt
Title title = new Title() { TitleText = titleText };

// Initiera Sidklassobjekt
Page page = new Note.Page() { Title = title };

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Se även

* class [Style](../style/)
* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


