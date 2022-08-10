---
title: Title
second_title: Aspose.Note för .NET API-referens
description: Representerar en titel.
type: docs
weight: 950
url: /sv/net/aspose.note/title/
---
## Title class

Representerar en titel.

```csharp
public sealed class Title : CompositeNodeBase, ICompositeNode<RichText>, IPageChildNode
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Title](title#constructor)() | Initierar en ny instans av[`Title`](../title) class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Document](../../aspose.note/node/document) { get; } | Hämtar dokumentet för noden. |
| [HorizontalOffset](../../aspose.note/title/horizontaloffset) { get; set; } | Hämtar eller ställer in den horisontella offseten. |
| override [IsComposite](../../aspose.note/title/iscomposite) { get; } | Får ett värde som indikerar om denna nod är sammansatt. Om sant kan noden ha underordnade noder. |
| [LastModifiedTime](../../aspose.note/title/lastmodifiedtime) { get; set; } | Hämtar eller ställer in den senast ändrade tiden. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Hämtar nodtypen. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Hämtar föregående nod på samma nodträdsnivå. |
| [TitleDate](../../aspose.note/title/titledate) { get; set; } | Hämtar eller ställer in en strängrepresentation av datumet i titeln. |
| [TitleText](../../aspose.note/title/titletext) { get; set; } | Hämtar eller ställer in texten i titeln. |
| [TitleTime](../../aspose.note/title/titletime) { get; set; } | Hämtar eller ställer in en strängrepresentation av tiden i titeln. |
| [VerticalOffset](../../aspose.note/title/verticaloffset) { get; set; } | Hämtar eller ställer in den vertikala offseten. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/title/accept)(DocumentVisitor) | Accepterar besökaren av noden. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/title/getchildnodes#getchildnodes_1)() | Hämta alla underordnade noder efter nodtyp. |
| [GetEnumerator](../../aspose.note/title/getenumerator)() | Returnerar en enumerator som itererar genom underordnade noder av[`Title`](../title) . |

### Exempel

Visar hur man redigerar sidans historik.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument och skaffa första barn           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Visar hur man ställer in en titel för en sida.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

Visar hur man skapar ett dokument och sparar det i html-format med standardalternativ.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initiera OneNote-dokument
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Spara i HTML-format
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Visar hur man skapar ett dokument och sparar i html-format specificerat antal sidor.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initiera OneNote-dokument
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Spara i HTML-format
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Visar hur man skapar ett dokument med titelsida.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Skapa ett objekt av klassen Document
Document doc = new Aspose.Note.Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Ställ in sidtitelegenskaper
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Lägg till sidnod i dokumentet
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Visar hur man sparar ett dokument i olika format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initiera det nya dokumentet
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initiera den nya sidan
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument i olika format, ställ in textstorlek och upptäck layoutändringar manuellt.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Se även

* class [CompositeNodeBase](../compositenodebase)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1)
* class [RichText](../richtext)
* interface [IPageChildNode](../ipagechildnode)
* namnutrymme [Aspose.Note](../../aspose.note)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
