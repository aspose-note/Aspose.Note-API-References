---
title: Class TextStyle
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.TextStyle classe. Specifica lo stile del testo.
type: docs
weight: 970
url: /it/net/aspose.note/textstyle/
---
## TextStyle class

Specifica lo stile del testo.

```csharp
public sealed class TextStyle : Style
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TextStyle](textstyle/)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default/) { get; } | Ottiene lo stile con la cultura "en-US". |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle/) { get; } | Ottiene lo stile predefinito per la data del titolo in MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle/) { get; } | Ottiene lo stile predefinito per il testo del titolo in MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle/) { get; } | Ottiene lo stile predefinito per l'ora del titolo in MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Ottiene o imposta il colore del carattere. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Ottiene o imposta il nome del font. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Ottiene o imposta la dimensione del carattere. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Ottiene lo stile del carattere. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Ottiene o imposta il colore di evidenziazione. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress/) { get; set; } | Ottiene o imposta l'indirizzo del collegamento ipertestuale. Deve essere impostato se il valore di[`IsHyperlink`](./ishyperlink/) proprietà è true. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è in grassetto. |
| [IsHidden](../../aspose.note/textstyle/ishidden/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è nascosto. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è collegamento ipertestuale. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è corsivo. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è di formattazione matematica. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è barrato. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è pedice. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è apice. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è sottolineato. |
| [Language](../../aspose.note/textstyle/language/) { get; set; } | Ottiene o imposta la lingua del testo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals/#equals_1)(object) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| [Equals](../../aspose.note/textstyle/equals/#equals)(TextStyle) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode/)() | Funge da funzione hash per il tipo. |

### Esempi

Mettiamo in risalto i titoli delle pagine tra le altre intestazioni aumentando la dimensione del carattere.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Itera attraverso i titoli della pagina.
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

Sottolineiamo le ultime modifiche al testo evidenziando.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Ottieni i nodi RichText modificati la scorsa settimana.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Imposta il colore di evidenziazione
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Imposta il colore di evidenziazione
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Imposta la lingua di correzione per un testo.

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

Manipolare in base al formato del testo utilizzando lo stile di paragrafo.

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

Mostra come associare un collegamento ipertestuale a un testo.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tasks();

// Crea un oggetto della classe Document
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

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem);

// Inizializza l'oggetto della classe Title
Title title = new Title() { TitleText = titleText };

// Inizializza l'oggetto della classe Page
Page page = new Note.Page() { Title = title };

// Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi nodo Pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Guarda anche

* class [Style](../style/)
* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


