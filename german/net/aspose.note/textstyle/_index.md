---
title: TextStyle
second_title: Aspose.Note für .NET-API-Referenz
description: Gibt den Textstil an.
type: docs
weight: 940
url: /de/net/aspose.note/textstyle/
---
## TextStyle class

Gibt den Textstil an.

```csharp
public sealed class TextStyle : Style
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [TextStyle](textstyle)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default) { get; } | Ruft den Standardstil für Titeltext in MS OneNote ab. |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle) { get; } | Ruft den Standardstil für das Titeldatum in MS OneNote ab. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle) { get; } | Ruft den Standardstil für Titeltext in MS OneNote ab. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle) { get; } | Ruft den Standardstil für die Titelzeit in MS OneNote ab. |
| [FontColor](../../aspose.note/style/fontcolor) { get; set; } | Ruft die Schriftfarbe ab oder legt sie fest. |
| [FontName](../../aspose.note/style/fontname) { get; set; } | Ruft den Schriftartnamen ab oder legt ihn fest. |
| [FontSize](../../aspose.note/style/fontsize) { get; set; } | Ruft die Schriftgröße ab oder legt sie fest. |
| [FontStyle](../../aspose.note/style/fontstyle) { get; } | Ruft den Schriftstil ab. |
| [Highlight](../../aspose.note/style/highlight) { get; set; } | Ruft die Hervorhebungsfarbe ab oder legt sie fest. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress) { get; set; } | Ruft die Hyperlink-Adresse ab oder legt sie fest. Muss gesetzt werden, wenn der Wert der[`IsHyperlink`](./ishyperlink) Eigenschaft ist wahr. |
| [IsBold](../../aspose.note/style/isbold) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil fett ist. |
| [IsHidden](../../aspose.note/textstyle/ishidden) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil ausgeblendet ist. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil ein Hyperlink ist. |
| [IsItalic](../../aspose.note/style/isitalic) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil kursiv ist. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil mathematisch formatiert ist. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil durchgestrichen ist. |
| [IsSubscript](../../aspose.note/style/issubscript) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil tiefgestellt ist. |
| [IsSuperscript](../../aspose.note/style/issuperscript) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil hochgestellt ist. |
| [IsUnderline](../../aspose.note/style/isunderline) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil unterstrichen ist. |
| [Language](../../aspose.note/textstyle/language) { get; set; } | Holt oder setzt die Sprache des Textes. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals#equals_1)(object) | Bestimmt, ob das angegebene Objekt gleich dem aktuellen Objekt ist. |
| [Equals](../../aspose.note/textstyle/equals#equals)(TextStyle) | Bestimmt, ob das angegebene Objekt gleich dem aktuellen Objekt ist. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode)() | dient als Hash-Funktion für den Typ. |

### Beispiele

Lassen Sie uns die Seitentitel unter anderen Überschriften hervorheben, indem wir die Schriftgröße erhöhen.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Seitentitel durchlaufen.
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

Lassen Sie uns die Änderungen des letzten Textes hervorheben, indem wir sie hervorheben.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// RichText-Knoten abrufen, die letzte Woche geändert wurden.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Hervorhebungsfarbe setzen
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Hervorhebungsfarbe setzen
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Legen Sie die Korrektursprache für einen Text fest.

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

Bearbeiten nach Textformat mit Absatzstil.

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

Zeigt, wie ein Hyperlink an einen Text gebunden wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tasks();

// Erstellen Sie ein Objekt der Document-Klasse
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

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem);

// Titelklassenobjekt initialisieren
Title title = new Title() { TitleText = titleText };

// Seitenklassenobjekt initialisieren
Page page = new Note.Page() { Title = title };

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Siehe auch

* class [Style](../style)
* namensraum [Aspose.Note](../../aspose.note)
* Montage [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
