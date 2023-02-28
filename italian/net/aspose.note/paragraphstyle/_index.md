---
title: Class ParagraphStyle
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.ParagraphStyle classe. Impostazioni dello stile del testo da utilizzare se non è presente alcun oggetto TextStyle corrispondenteStyles collection o questo oggetto non specifica unimpostazione necessaria.
type: docs
weight: 510
url: /it/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

Impostazioni dello stile del testo da utilizzare se non è presente alcun oggetto TextStyle corrispondenteStyles collection o questo oggetto non specifica un'impostazione necessaria.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | Inizializza una nuova istanza di`ParagraphStyle` classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | Ottiene il ParagraphStyle con le impostazioni predefinite. |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | Ottiene o imposta il colore del carattere. |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | Ottiene o imposta il nome del font. |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | Ottiene o imposta la dimensione del carattere. |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | Ottiene lo stile del carattere. |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | Ottiene o imposta il colore di evidenziazione. |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è in grassetto. |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è corsivo. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è barrato. |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è pedice. |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è apice. |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | Ottiene o imposta un valore che indica se lo stile del testo è sottolineato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | Funge da funzione hash per il tipo. |

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

Mostra come inserire una nuova lista con numerazione cinese.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Inizializza il documento OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// Inizializza la pagina di OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Applica le impostazioni dello stile del testo
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// I numeri nella stessa struttura vengono incrementati automaticamente.
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

// Salva documento OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Mostra come inserire nuovi elenchi puntati.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crea un oggetto della classe Document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe TextStyle e imposta le proprietà di formattazione
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inizializza gli oggetti della classe OutlineElement e applica i punti elenco
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Inizializza l'oggetto della classe RichText e applica lo stile del testo
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Aggiungi nodo Struttura
page.AppendChildLast(outline);
// Aggiungi nodo Pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Mostra come inserire una nuova lista con numerazione.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto della classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto della classe TextStyle e imposta le proprietà di formattazione
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inizializza gli oggetti della classe OutlineElement e applica la numerazione
// I numeri nella stessa struttura vengono incrementati automaticamente.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Aggiungi elementi di contorno
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi nodo Pagina
doc.AppendChildLast(page);

// Salva documento OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Guarda anche

* class [Style](../style/)
* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


