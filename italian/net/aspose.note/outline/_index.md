---
title: Outline
second_title: Aspose.Note per .NET API Reference
description: Rappresenta un contorno.
type: docs
weight: 430
url: /it/net/aspose.note/outline/
---
## Outline class

Rappresenta un contorno.

```csharp
public sealed class Outline : CompositeNode<IOutlineChildNode>, IPageChildNode
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Outline](outline#constructor)() | Inizializza una nuova istanza di[`Outline`](../outline) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DescendantsCannotBeMoved](../../aspose.note/outline/descendantscannotbemoved) { get; set; } | Ottiene se è possibile spostare i discendenti del profilo. |
| [Document](../../aspose.note/node/document) { get; } | Ottiene il documento del nodo. |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [HorizontalOffset](../../aspose.note/outline/horizontaloffset) { get; set; } | Ottiene o imposta l'offset orizzontale. |
| [IndentPosition](../../aspose.note/outline/indentposition) { get; set; } | Ottiene o imposta la posizione del rientro. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/outline/lastmodifiedtime) { get; set; } | Ottiene o imposta l'ultima ora modificata. |
| [MaxHeight](../../aspose.note/outline/maxheight) { get; set; } | Ottiene o imposta l'altezza massima. |
| [MaxWidth](../../aspose.note/outline/maxwidth) { get; set; } | Ottiene o imposta la larghezza massima. |
| [MinWidth](../../aspose.note/outline/minwidth) { get; set; } | Ottiene o imposta la larghezza minima. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Ottiene il nodo successivo allo stesso livello di albero dei nodi. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Ottiene il tipo di nodo. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Ottiene il nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Ottiene il nodo precedente allo stesso livello di albero dei nodi. |
| [ReservedWidth](../../aspose.note/outline/reservedwidth) { get; set; } | Ottiene o imposta la larghezza riservata. |
| [VerticalOffset](../../aspose.note/outline/verticaloffset) { get; set; } | Ottiene o imposta l'offset verticale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Accept](../../aspose.note/outline/accept)(DocumentVisitor) | Accetta il visitatore del nodo. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### Esempi

Mostra come aggiungere una nuova immagine con tag.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe Pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inizializza l'oggetto classe Outline
Outline outline = new Outline(doc);

// Inizializza l'oggetto classe OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Carica un'immagine
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Inserisce l'immagine nel nodo del documento
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Aggiunge il nodo dell'elemento struttura
outline.AppendChildLast(outlineElem);

// Aggiungi nodo struttura
page.AppendChildLast(outline);

// Aggiungi il nodo della pagina
doc.AppendChildLast(page);

// Salva il documento di OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
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

### Guarda anche

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* interface [IOutlineChildNode](../ioutlinechildnode)
* interface [IPageChildNode](../ipagechildnode)
* spazio dei nomi [Aspose.Note](../../aspose.note)
* assemblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
