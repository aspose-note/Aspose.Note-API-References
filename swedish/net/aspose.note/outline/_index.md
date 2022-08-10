---
title: Outline
second_title: Aspose.Note för .NET API-referens
description: Representerar en disposition.
type: docs
weight: 430
url: /sv/net/aspose.note/outline/
---
## Outline class

Representerar en disposition.

```csharp
public sealed class Outline : CompositeNode<IOutlineChildNode>, IPageChildNode
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Outline](outline#constructor)() | Initierar en ny instans av[`Outline`](../outline) class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [DescendantsCannotBeMoved](../../aspose.note/outline/descendantscannotbemoved) { get; set; } | Hämtar om ättlingar till konturen kan flyttas. |
| [Document](../../aspose.note/node/document) { get; } | Hämtar dokumentet för noden. |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [HorizontalOffset](../../aspose.note/outline/horizontaloffset) { get; set; } | Hämtar eller ställer in den horisontella offseten. |
| [IndentPosition](../../aspose.note/outline/indentposition) { get; set; } | Hämtar eller ställer in indragspositionen. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/outline/lastmodifiedtime) { get; set; } | Hämtar eller ställer in den senast ändrade tiden. |
| [MaxHeight](../../aspose.note/outline/maxheight) { get; set; } | Hämtar eller ställer in maxhöjden. |
| [MaxWidth](../../aspose.note/outline/maxwidth) { get; set; } | Hämtar eller ställer in maxbredden. |
| [MinWidth](../../aspose.note/outline/minwidth) { get; set; } | Hämtar eller ställer in min bredd. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Hämtar nodtypen. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Hämtar föregående nod på samma nodträdsnivå. |
| [ReservedWidth](../../aspose.note/outline/reservedwidth) { get; set; } | Hämtar eller ställer in den reserverade bredden. |
| [VerticalOffset](../../aspose.note/outline/verticaloffset) { get; set; } | Hämtar eller ställer in den vertikala offseten. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/outline/accept)(DocumentVisitor) | Accepterar besökaren av noden. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### Exempel

Visar hur man lägger till ny bild med tagg.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tags();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjekt
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

// Ladda en bild
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Infoga bild i dokumentnoden
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Lägg till nod för dispositionselement
outline.AppendChildLast(outlineElem);

// Lägg till dispositionsnod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

Visar hur man infogar en ny lista med kinesisk numrering.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Initiera OneNote-dokument
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initiera OneNote-sidan
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Använd textstilsinställningar
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Siffror i samma disposition ökas automatiskt.
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

// Spara OneNote-dokument
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Visar hur man infogar ny punktlista.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Skapa ett objekt av klassen Document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjekt
Outline outline = new Outline(doc);

// Initiera TextStyle-klassobjektet och ställ in formateringsegenskaper
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initiera OutlineElement-klassobjekt och använd kulor
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Initiera RichText-klassobjekt och tillämpa textstil
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Lägg till konturelement
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Lägg till Outline-nod
page.AppendChildLast(outline);
// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Visar hur man infogar en ny lista med numrering.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjekt
Outline outline = new Outline(doc);

// Initiera TextStyle-klassobjektet och ställ in formateringsegenskaper
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initiera OutlineElement-klassobjekt och tillämpa numrering
// Siffror i samma disposition ökas automatiskt.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Lägg till konturelement
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Se även

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* interface [IOutlineChildNode](../ioutlinechildnode)
* interface [IPageChildNode](../ipagechildnode)
* namnutrymme [Aspose.Note](../../aspose.note)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
