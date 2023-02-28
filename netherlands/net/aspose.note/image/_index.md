---
title: Class Image
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Image klas. Vertegenwoordigt een afbeelding.
type: docs
weight: 250
url: /nl/net/aspose.note/image/
---
## Image class

Vertegenwoordigt een afbeelding.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Image](image/#constructor)() | Initialiseert een nieuw exemplaar van het`Image` klasse. |
| [Image](image/#constructor_4)(string, Stream) | Initialiseert een nieuw exemplaar van het`Image` klasse. |
| [Image](image/#constructor_5)(string, string, string) | Initialiseert een nieuw exemplaar van het`Image` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | Haalt of stelt de uitlijning in. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | Krijgt of stelt een body in als alternatieve tekst voor de afbeelding. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | Haalt of stelt een titel van alternatieve tekst voor de afbeelding in. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | Haalt de afbeeldingsgegevensopslag op. |
| [Document](../../aspose.note/node/document/) { get; } | Haalt het document van het knooppunt op. |
| [FileName](../../aspose.note/image/filename/) { get; } | Krijgt de bestandsnaam. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | Haalt het pad naar het afbeeldingsbestand op. |
| [Format](../../aspose.note/image/format/) { get; } | Haalt het formaat van de afbeelding op. |
| [Height](../../aspose.note/image/height/) { get; set; } | Haalt of stelt de hoogte in. Dit is de werkelijke hoogte van de afbeelding in het MS OneNote-document. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | Haalt of stelt de horizontale offset in. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | Haalt of stelt de hyperlink in die aan de afbeelding is gekoppeld. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | Krijgt of de afbeelding een achtergrondafbeelding is. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Krijgt een waarde die aangeeft of dit knooppunt samengesteld is. Indien waar, kan het knooppunt onderliggende knooppunten hebben. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | Haalt of stelt de laatst gewijzigde tijd in. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Haalt het volgende knooppunt op op hetzelfde knooppuntboomniveau. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Haalt het knooppunttype op. |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | Krijgt de oorspronkelijke hoogte. Dit is de oorspronkelijke breedte van de afbeelding, voordat de grootte wordt gewijzigd. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | Krijgt de oorspronkelijke breedte. Dit is de oorspronkelijke breedte van de afbeelding, voordat de grootte wordt gewijzigd. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Haalt het bovenliggende knooppunt op. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Haalt het vorige knooppunt op hetzelfde knooppuntboomniveau. |
| [Tags](../../aspose.note/image/tags/) { get; } | Krijgt de lijst met alle tags van een paragraaf. |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | Haalt of stelt de verticale offset in. |
| [Width](../../aspose.note/image/width/) { get; set; } | Haalt of stelt de breedte in. Dit is de werkelijke breedte van de afbeelding in het MS OneNote-document. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | Accepteert de bezoeker van de node. |

### Voorbeelden

Laat zien hoe u een hyperlink aan een afbeelding koppelt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://afbeelding.com"};

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Laat zien hoe u een tekstbeschrijving voor een afbeelding instelt.

```csharp
// Het pad naar de documentenmap.
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

Laat zien hoe u een afbeelding uit een document haalt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle afbeeldingsknooppunten op
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Bewaar afbeeldingsbytes in een bestand
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Laat zien hoe u de meta-informatie van de afbeelding kunt krijgen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle afbeeldingsknooppunten op
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

Laat zien hoe een nieuwe afbeelding met tag kan worden toegevoegd.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Laad een afbeelding
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Afbeelding invoegen in het documentknooppunt
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Voeg overzichtselementknooppunt toe
outline.AppendChildLast(outlineElem);

// Voeg overzichtsknooppunt toe
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een afbeelding uit een bestand toevoegt aan een document met door de gebruiker gedefinieerde eigenschappen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad document uit de stream.
Document doc = new Document(dataDir + "Aspose.one");

// Haal de eerste pagina van het document op.
Aspose.Note.Page page = doc.FirstChild;

// Laad een afbeelding uit het bestand.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Wijzig de grootte van de afbeelding volgens uw behoeften (optioneel).
                              Width = 100,
                              Height = 100,

                              // Stel de locatie van de afbeelding op de pagina in (optioneel).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Beelduitlijning instellen
                              Alignment = HorizontalAlignment.Right
                          };

// Voeg de afbeelding toe aan de pagina.
page.AppendChildLast(image);
```

Laat zien hoe u een afbeelding uit een stream toevoegt aan een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Laad de tweede afbeelding met de afbeeldingsnaam, extensie en stream.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Beelduitlijning instellen
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een afbeelding uit een bestand toevoegt aan een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klasseobject en stel offset-eigenschappen in
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Laad een afbeelding via het bestandspad.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Beelduitlijning instellen
                              Alignment = HorizontalAlignment.Right
                          };

// Voeg afbeelding toe
outlineElem.AppendChildLast(image);

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem);

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Zie ook

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


