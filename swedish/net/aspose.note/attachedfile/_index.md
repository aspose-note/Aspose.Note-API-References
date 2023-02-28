---
title: Class AttachedFile
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.AttachedFile klass. Representerar en bifogad fil.
type: docs
weight: 10
url: /sv/net/aspose.note/attachedfile/
---
## AttachedFile class

Representerar en bifogad fil.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [AttachedFile](attachedfile/#constructor)() | Initierar en ny instans av`AttachedFile` class. |
| [AttachedFile](attachedfile/#constructor_6)(string, Stream) | Initierar en ny instans av`AttachedFile` class. |
| [AttachedFile](attachedfile/#constructor_7)(string, Stream, ImageFormat) | Initierar en ny instans av`AttachedFile` class. |
| [AttachedFile](attachedfile/#constructor_8)(string, Stream, Stream, ImageFormat) | Initierar en ny instans av`AttachedFile` class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment/) { get; set; } | Hämtar eller ställer in justeringen. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription/) { get; set; } | Hämtar eller ställer in en text som alternativ text för ikonen för den bifogade filen. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle/) { get; set; } | Hämtar eller ställer in en titel på alternativ text för ikonen för den bifogade filen. |
| [Bytes](../../aspose.note/attachedfile/bytes/) { get; } | Hämtar binära data för en inbäddad fil. |
| [Document](../../aspose.note/node/document/) { get; } | Hämtar dokumentet för noden. |
| [Extension](../../aspose.note/attachedfile/extension/) { get; } | Hämtar tillägget av en inbäddad fil. |
| [FileName](../../aspose.note/attachedfile/filename/) { get; } | Hämtar namnet på den inbäddade filen. |
| [FilePath](../../aspose.note/attachedfile/filepath/) { get; } | Hämtar sökvägen till originalfilen. |
| [Height](../../aspose.note/attachedfile/height/) { get; } | Får den ursprungliga höjden på den inbäddade filikonen. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset/) { get; set; } | Hämtar eller ställer in den horisontella offseten. |
| [Icon](../../aspose.note/attachedfile/icon/) { get; } | Hämtar binär data för ikonen som är associerad med den inbäddade filen. |
| [IconExtension](../../aspose.note/attachedfile/iconextension/) { get; } | Hämtar förlängningen av ikonen. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Får ett värde som indikerar om denna nod är sammansatt. Om sant kan noden ha underordnade noder. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout/) { get; set; } | Hämtar eller ställer in ett värde som anger om vyn av filen är utskrift. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser/) { get; set; } | Hämtar eller ställer in ett värde som indikerar om värdet på ikonens storlek uttryckligen har uppdaterats av användaren. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime/) { get; set; } | Hämtar eller ställer in den senast ändrade tiden. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight/) { get; set; } | Hämtar eller ställer in maximal höjd för att visa den inbäddade filikonen. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth/) { get; set; } | Hämtar eller ställer in maximal bredd för att visa den inbäddade filikonen. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Hämtar nodtypen. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Hämtar föregående nod på samma nodträdsnivå. |
| [Tags](../../aspose.note/attachedfile/tags/) { get; } | Hämtar listan över alla taggar i ett stycke. |
| [Text](../../aspose.note/attachedfile/text/) { get; set; } | Hämtar eller ställer in textrepresentationen för den inbäddade filen. Strängen FÅR INTE innehålla några tecken med värdet 10 (radmatning) eller 13 (vagnretur). |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset/) { get; set; } | Hämtar eller ställer in den vertikala offseten. |
| [Width](../../aspose.note/attachedfile/width/) { get; } | Får den ursprungliga bredden på den inbäddade filikonen. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept/)(DocumentVisitor) | Accepterar besökaren av noden. |

### Exempel

Visar hur man får innehållet i en bifogad fil.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Få en lista över bifogade filnoder
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Iterera genom alla noder
foreach (AttachedFile file in nodes)
{
    // Ladda bifogad fil till ett strömobjekt
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Skapa en lokal fil
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Kopiera filström
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Visar hur man lägger till en fil i ett dokument med hjälp av filsökväg.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjekt
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

// Initiera AttachedFile-klassobjektet
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Lägg till bifogad fil
outlineElem.AppendChildLast(attachedFile);

// Lägg till nod för dispositionselement
outline.AppendChildLast(outlineElem);

// Lägg till dispositionsnod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Visar hur man lägger till en fil från en ström till ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Attachments();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjekt
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Initiera AttachedFile-klassobjektet och skicka även dess ikonsökväg
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Lägg till bifogad fil
    outlineElem.AppendChildLast(attachedFile);
}

// Lägg till nod för dispositionselement
outline.AppendChildLast(outlineElem);

// Lägg till dispositionsnod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### Se även

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


