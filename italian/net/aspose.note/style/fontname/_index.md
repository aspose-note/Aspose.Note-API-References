---
title: FontName
second_title: Aspose.Note per .NET API Reference
description: Ottiene o imposta il nome del carattere.
type: docs
weight: 20
url: /it/net/aspose.note/style/fontname/
---
## Style.FontName property

Ottiene o imposta il nome del carattere.

```csharp
public string FontName { get; set; }
```

### Esempi

Manipola in base al formato del testo usando lo stile di paragrafo.

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

//---------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//---------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//---------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Mostra come inserire nuovi elenchi puntati.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crea un oggetto della classe Document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto classe TextStyle e imposta le proprietà di formattazione
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

//Aggiungi nodo Struttura
page.AppendChildLast(outline);
// Aggiungi il nodo Pagina
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Mostra come inserire una nuova lista con numerazione.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto classe TextStyle e imposta le proprietà di formattazione
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

//Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi il nodo Pagina
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
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

// Inizializza l'oggetto della classe Pagina
Page page = new Note.Page() { Title = title };

//Aggiungi nodo Struttura
page.AppendChildLast(outline);

// Aggiungi il nodo Pagina
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Guarda anche

* class [Style](../../style)
* spazio dei nomi [Aspose.Note](../../style)
* assemblea [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
