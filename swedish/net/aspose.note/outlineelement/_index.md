---
title: OutlineElement
second_title: Aspose.Note för .NET API-referens
description: Representerar ett konturelement.
type: docs
weight: 440
url: /sv/net/aspose.note/outlineelement/
---
## OutlineElement class

Representerar ett konturelement.

```csharp
public sealed class OutlineElement : CompositeNode<IOutlineElementChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [OutlineElement](outlineelement#constructor)() | Initierar en ny instans av[`OutlineElement`](../outlineelement) class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [CreationTime](../../aspose.note/outlineelement/creationtime) { get; set; } | Hämtar eller ställer in skapelsetiden. |
| [Document](../../aspose.note/node/document) { get; } | Hämtar dokumentet för noden. |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IndentPosition](../../aspose.note/outlineelement/indentposition) { get; set; } | Hämtar eller ställer in indragspositionen. |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/outlineelement/lastmodifiedtime) { get; set; } | Hämtar eller ställer in den senast ändrade tiden. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Hämtar nodtypen. |
| [NumberList](../../aspose.note/outlineelement/numberlist) { get; set; } | Hämtar eller ställer in stilen för den numrerade listhuvudet. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Hämtar föregående nod på samma nodträdsnivå. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/outlineelement/accept)(DocumentVisitor) | Accepterar besökaren av noden. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;IOutlineElementChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params IOutlineElementChildNode[]) |  |
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

Visar hur man hämtar information om listans formatering.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Hämta en samling noder av konturelementet
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Iterera genom varje nod
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Hämta teckensnittsnamn
        Console.WriteLine("Font Name: " + list.Font);

        // Hämta teckensnittslängd
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Hämta teckenstorlek
        Console.WriteLine("Font Size: " + list.FontSize);

        // Hämta teckensnittsfärg
        Console.WriteLine("Font Color: " + list.FontColor);

        // Hämta format
        Console.WriteLine("Font format: " + list.Format);

        // Markera fetstil
        Console.WriteLine("Is bold: " + list.IsBold);

        // Markera kursiv
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
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
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IOutlineChildNode](../ioutlinechildnode)
* namnutrymme [Aspose.Note](../../aspose.note)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
