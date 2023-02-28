---
title: Class AttachedFile
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.AttachedFile klas. Vertegenwoordigt een bijgevoegd bestand.
type: docs
weight: 10
url: /nl/net/aspose.note/attachedfile/
---
## AttachedFile class

Vertegenwoordigt een bijgevoegd bestand.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [AttachedFile](attachedfile/#constructor)() | Initialiseert een nieuw exemplaar van het`AttachedFile` klasse. |
| [AttachedFile](attachedfile/#constructor_6)(string, Stream) | Initialiseert een nieuw exemplaar van het`AttachedFile` klasse. |
| [AttachedFile](attachedfile/#constructor_7)(string, Stream, ImageFormat) | Initialiseert een nieuw exemplaar van het`AttachedFile` klasse. |
| [AttachedFile](attachedfile/#constructor_8)(string, Stream, Stream, ImageFormat) | Initialiseert een nieuw exemplaar van het`AttachedFile` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment/) { get; set; } | Haalt of stelt de uitlijning in. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription/) { get; set; } | Haalt of stelt een body in een alternatieve tekst voor het pictogram van het bijgevoegde bestand. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle/) { get; set; } | Haalt of stelt een titel van alternatieve tekst in voor het pictogram van het bijgevoegde bestand. |
| [Bytes](../../aspose.note/attachedfile/bytes/) { get; } | Haalt de binaire gegevens op voor een ingesloten bestand. |
| [Document](../../aspose.note/node/document/) { get; } | Haalt het document van het knooppunt op. |
| [Extension](../../aspose.note/attachedfile/extension/) { get; } | Krijgt de extensie van een ingesloten bestand. |
| [FileName](../../aspose.note/attachedfile/filename/) { get; } | Krijgt de naam van het ingesloten bestand. |
| [FilePath](../../aspose.note/attachedfile/filepath/) { get; } | Haalt het pad naar het oorspronkelijke bestand op. |
| [Height](../../aspose.note/attachedfile/height/) { get; } | Hiermee krijgt u de oorspronkelijke hoogte van het ingesloten bestandspictogram. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset/) { get; set; } | Haalt of stelt de horizontale offset in. |
| [Icon](../../aspose.note/attachedfile/icon/) { get; } | Haalt de binaire gegevens op voor het pictogram dat is gekoppeld aan het ingesloten bestand. |
| [IconExtension](../../aspose.note/attachedfile/iconextension/) { get; } | Krijgt de extensie van het pictogram. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Krijgt een waarde die aangeeft of dit knooppunt samengesteld is. Indien waar, kan het knooppunt onderliggende knooppunten hebben. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout/) { get; set; } | Haalt of stelt een waarde in die aangeeft of de weergave van het bestand afdrukbaar is. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser/) { get; set; } | Haalt of stelt een waarde in die aangeeft of de waarde van de grootte van het pictogram expliciet is bijgewerkt door de gebruiker. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime/) { get; set; } | Haalt of stelt de laatst gewijzigde tijd in. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight/) { get; set; } | Haalt of stelt de maximale hoogte in om het ingesloten bestandspictogram weer te geven. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth/) { get; set; } | Haalt of stelt de maximale breedte in om het ingesloten bestandspictogram weer te geven. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Haalt het volgende knooppunt op op hetzelfde knooppuntboomniveau. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Haalt het knooppunttype op. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Haalt het bovenliggende knooppunt op. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Haalt het vorige knooppunt op hetzelfde knooppuntboomniveau. |
| [Tags](../../aspose.note/attachedfile/tags/) { get; } | Krijgt de lijst met alle tags van een paragraaf. |
| [Text](../../aspose.note/attachedfile/text/) { get; set; } | Haalt of stelt de tekstrepresentatie van het ingesloten bestand in. De tekenreeks MAG GEEN tekens bevatten met de waarde 10 (regelinvoer) of 13 (regelterugloop). |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset/) { get; set; } | Haalt of stelt de verticale offset in. |
| [Width](../../aspose.note/attachedfile/width/) { get; } | Krijgt de oorspronkelijke breedte van het ingesloten bestandspictogram. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept/)(DocumentVisitor) | Accepteert de bezoeker van de node. |

### Voorbeelden

Laat zien hoe u de inhoud van een bijgevoegd bestand kunt ophalen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Attachments();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Krijg een lijst met bijgevoegde bestandsknooppunten
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Doorloop alle knooppunten
foreach (AttachedFile file in nodes)
{
    // Laad bijgevoegd bestand naar een streamobject
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Maak een lokaal bestand
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Bestandsstroom kopiëren
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Laat zien hoe een bestand aan een document kan worden toegevoegd met behulp van bestandspad.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Attachments();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Initialiseer het klasseobject AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Voeg bijgevoegd bestand toe
outlineElem.AppendChildLast(attachedFile);

// Voeg overzichtselementknooppunt toe
outline.AppendChildLast(outlineElem);

// Voeg overzichtsknooppunt toe
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een bestand uit een stroom toevoegt aan een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Attachments();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Initialiseer het klasseobject AttachedFile en geef ook het pictogrampad door
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Voeg bijgevoegd bestand toe
    outlineElem.AppendChildLast(attachedFile);
}

// Voeg overzichtselementknooppunt toe
outline.AppendChildLast(outlineElem);

// Voeg overzichtsknooppunt toe
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### Zie ook

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


