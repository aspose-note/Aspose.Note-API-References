---
title: Class ParagraphStyle
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.ParagraphStyle klas. Zu verwendende Textstileinstellungen wenn kein passendes TextStyleObjekt vorhanden istStyles entweder dieses Objekt gibt keine erforderliche Einstellung an.
type: docs
weight: 510
url: /de/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

Zu verwendende Textstileinstellungen, wenn kein passendes TextStyle-Objekt vorhanden istStyles entweder dieses Objekt gibt keine erforderliche Einstellung an.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | Initialisiert eine neue Instanz von`ParagraphStyle` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | Ruft den ParagraphStyle mit Standardeinstellungen ab. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Ruft die Schriftfarbe ab oder legt sie fest. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Ruft den Schriftartnamen ab oder legt ihn fest. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Ruft die Schriftgröße ab oder legt sie fest. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Ruft den Schriftstil ab. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Ruft die Hervorhebungsfarbe ab oder legt sie fest. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil fett ist. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil kursiv ist. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil durchgestrichen ist. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil tiefgestellt ist. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil hochgestellt ist. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Textstil unterstrichen ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | Bestimmt, ob das angegebene Objekt gleich dem aktuellen Objekt ist. |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | Bestimmt, ob das angegebene Objekt gleich dem aktuellen Objekt ist. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | dient als Hash-Funktion für den Typ. |

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

Zeigt, wie eine neue Liste mit chinesischer Nummerierung eingefügt wird.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// OneNote-Dokument initialisieren
Aspose.Note.Document doc = new Aspose.Note.Document();

// OneNote-Seite initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Textstileinstellungen anwenden
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Zahlen in derselben Gliederung werden automatisch erhöht.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Zeigt, wie neue Listen mit Aufzählungszeichen eingefügt werden.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Erstellen Sie ein Objekt der Document-Klasse
Aspose.Note.Document doc = new Aspose.Note.Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// TextStyle-Klassenobjekt initialisieren und Formatierungseigenschaften festlegen
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Objekte der OutlineElement-Klasse initialisieren und Aufzählungszeichen anwenden
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// RichText-Klassenobjekt initialisieren und Textstil anwenden
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);
// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Zeigt, wie eine neue Liste mit Nummerierung eingefügt wird.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// TextStyle-Klassenobjekt initialisieren und Formatierungseigenschaften festlegen
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Objekte der OutlineElement-Klasse initialisieren und Nummerierung anwenden
// Zahlen in derselben Gliederung werden automatisch erhöht.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Siehe auch

* class [Style](../style/)
* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


