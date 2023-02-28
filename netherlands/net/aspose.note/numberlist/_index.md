---
title: Class NumberList
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.NumberList klas. Vertegenwoordigt de genummerde lijst of lijst met opsommingstekens.
type: docs
weight: 440
url: /nl/net/aspose.note/numberlist/
---
## NumberList class

Vertegenwoordigt de genummerde lijst of lijst met opsommingstekens.

```csharp
public class NumberList
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | Initialiseert een nieuw exemplaar van het`NumberList`class. Deze instantie vertegenwoordigt een lijst met opsommingstekens. |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | Initialiseert een nieuw exemplaar van het`NumberList` class. Deze instantie vertegenwoordigt een genummerde lijst. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | Haalt de naam van het lettertype op of stelt deze in. |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | Hiermee wordt de letterkleur opgehaald of ingesteld. |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | Hiermee wordt de lettergrootte opgehaald of ingesteld. |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | Haalt de opmaak van de regelkop op of stelt deze in. Voor lijsten met opsommingstekens vertegenwoordigt een opsommingsteken. |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl vet is. |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl cursief is. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | Haalt of stelt de laatst gewijzigde tijd in. |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | Hiermee wordt de getalnotatie opgehaald of ingesteld die wordt gebruikt voor een groep automatisch genummerde objecten. Moet null zijn voor lijsten met opsommingstekens. |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | Hiermee wordt de numerieke waarde opgehaald of ingesteld die de automatische nummerwaarde van het lijstitem overschrijft. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | Dient als hash-functie voor het type. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | Haalt de genummerde lijstkop op. |

### Voorbeelden

Laat zien hoe informatie over de opmaak van de lijst kan worden opgehaald.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Haal een verzameling knooppunten van het overzichtselement op
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Doorloop elk knooppunt
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Lettertypenaam ophalen
        Console.WriteLine("Font Name: " + list.Font);

        // Letterlengte ophalen
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Lettergrootte ophalen
        Console.WriteLine("Font Size: " + list.FontSize);

        // Letterkleur ophalen
        Console.WriteLine("Font Color: " + list.FontColor);

        // Formaat ophalen
        Console.WriteLine("Font format: " + list.Format);

        // Vink vet aan
        Console.WriteLine("Is bold: " + list.IsBold);

        // Controleer cursief
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

Laat zien hoe u een nieuwe lijst met Chinese nummering invoegt.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Initialiseer OneNote-document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initialiseer de OneNote-pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Tekststijlinstellingen toepassen
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Getallen in dezelfde opbouw worden automatisch opgehoogd.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//---------------------------------------------------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//---------------------------------------------------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//---------------------------------------------------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Laat zien hoe u een nieuwe lijst met nummering invoegt.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject TextStyle en stel opmaakeigenschappen in
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialiseer de klasse-objecten van OutlineElement en pas nummering toe
// Getallen in dezelfde opbouw worden automatisch opgehoogd.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Zie ook

* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


