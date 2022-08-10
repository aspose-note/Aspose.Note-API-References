---
title: Image
second_title: Aspose.Note för .NET API-referens
description: Representerar en bild.
type: docs
weight: 240
url: /sv/net/aspose.note/image/
---
## Image class

Representerar en bild.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Image](image#constructor)() | Initierar en ny instans av[`Image`](../image) class. |
| [Image](image#constructor_4)(string, Stream) | Initierar en ny instans av[`Image`](../image) class. |
| [Image](image#constructor_5)(string, string, string) | Initierar en ny instans av[`Image`](../image) class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment) { get; set; } | Hämtar eller ställer in justeringen. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription) { get; set; } | Hämtar eller ställer in en text till en alternativ text för bilden. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle) { get; set; } | Hämtar eller ställer in en titel på alternativ text för bilden. |
| [Bytes](../../aspose.note/image/bytes) { get; } | Hämtar bilddatalagret. |
| [Document](../../aspose.note/node/document) { get; } | Hämtar dokumentet för noden. |
| [FileName](../../aspose.note/image/filename) { get; } | Hämtar filnamnet. |
| [FilePath](../../aspose.note/image/filepath) { get; } | Hämtar sökvägen till bildfilen. |
| [Format](../../aspose.note/image/format) { get; } | Hämtar bildens format. |
| [Height](../../aspose.note/image/height) { get; set; } | Hämtar eller ställer in höjden. Detta är den verkliga höjden på bilden i MS OneNote-dokumentet. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset) { get; set; } | Hämtar eller ställer in den horisontella offseten. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl) { get; set; } | Hämtar eller ställer in hyperlänken som är kopplad till bilden. |
| [IsBackground](../../aspose.note/image/isbackground) { get; set; } | Hämtar om bilden är en bakgrundsbild. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Får ett värde som indikerar om denna nod är sammansatt. Om sant kan noden ha underordnade noder. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime) { get; set; } | Hämtar eller ställer in senast ändrade tid. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Hämtar nodtypen. |
| [OriginalHeight](../../aspose.note/image/originalheight) { get; } | Får den ursprungliga höjden. Detta är bildens ursprungliga bredd innan storleksändring. |
| [OriginalWidth](../../aspose.note/image/originalwidth) { get; } | Får den ursprungliga bredden. Detta är bildens ursprungliga bredd innan storleksändring. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Hämtar föregående nod på samma nodträdsnivå. |
| [Tags](../../aspose.note/image/tags) { get; } | Hämtar listan över alla taggar i ett stycke. |
| [VerticalOffset](../../aspose.note/image/verticaloffset) { get; set; } | Hämtar eller ställer in den vertikala offseten. |
| [Width](../../aspose.note/image/width) { get; set; } | Hämtar eller ställer in bredden. Detta är den verkliga bredden på bilden i MS OneNote-dokumentet. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/image/accept)(DocumentVisitor) | Accepterar besökaren av noden. |

### Exempel

Visar hur man binder en hyperlänk till en bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Visar hur man ställer in textbeskrivning för en bild.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

Visar hur man hämtar en bild från ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta alla bildnoder
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Spara bildbytes till en fil
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Visar hur man får bildens metainformation.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta alla bildnoder
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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

Visar hur man lägger till en bild från fil till ett dokument med användardefinierade egenskaper.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Ladda dokument från strömmen.
Document doc = new Document(dataDir + "Aspose.one");

// Hämta den första sidan av dokumentet.
Aspose.Note.Page page = doc.FirstChild;

// Ladda en bild från filen.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ändra bildens storlek efter dina behov (valfritt).
                              Width = 100,
                              Height = 100,

                              // Ställ in bildens plats på sidan (valfritt).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Ställ in bildjustering
                              Alignment = HorizontalAlignment.Right
                          };

// Lägg till bilden på sidan.
page.AppendChildLast(image);
```

Visar hur man lägger till en bild från ström till ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Ladda den andra bilden med bildnamnet, tillägget och strömmen.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Ställ in bildjustering
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Visar hur man lägger till en bild från fil till ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjektet och ställ in offsetegenskaper
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

// Ladda en bild efter filsökvägen.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ställ in bildjustering
                              Alignment = HorizontalAlignment.Right
                          };

// Lägg till bild
outlineElem.AppendChildLast(image);

// Lägg till konturelement
outline.AppendChildLast(outlineElem);

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Se även

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* namnutrymme [Aspose.Note](../../aspose.note)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
