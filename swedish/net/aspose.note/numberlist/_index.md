---
title: NumberList
second_title: Aspose.Note för .NET API-referens
description: Representerar den numrerade eller punktlista.
type: docs
weight: 420
url: /sv/net/aspose.note/numberlist/
---
## NumberList class

Representerar den numrerade eller punktlista.

```csharp
public class NumberList
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [NumberList](numberlist#constructor_1)(string, string, int) | Initierar en ny instans av[`NumberList`](../numberlist) class. Den här instansen representerar en punktlista. |
| [NumberList](numberlist#constructor)(string, NumberFormat, string, int) | Initierar en ny instans av[`NumberList`](../numberlist)class. Denna instans representerar en numrerad lista. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Font](../../aspose.note/numberlist/font) { get; set; } | Hämtar eller ställer in namnet på teckensnittet. |
| [FontColor](../../aspose.note/numberlist/fontcolor) { get; set; } | Hämtar eller ställer in teckensnittsfärgen. |
| [FontSize](../../aspose.note/numberlist/fontsize) { get; set; } | Hämtar eller ställer in teckenstorleken. |
| [Format](../../aspose.note/numberlist/format) { get; set; } | Hämtar eller ställer in formatet på radhuvudet. För punktlistor representerar en punktsymbol. |
| [IsBold](../../aspose.note/numberlist/isbold) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är fetstil. |
| [IsItalic](../../aspose.note/numberlist/isitalic) { get; set; } | Hämtar eller ställer in ett värde som anger om textstilen är kursiv. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime) { get; set; } | Hämtar eller ställer in den senast ändrade tiden. |
| [NumberFormat](../../aspose.note/numberlist/numberformat) { get; set; } | Hämtar eller ställer in talformatet som används för en grupp av automatiskt numrerade objekt. Bör vara null för punktlistor. |
| [Restart](../../aspose.note/numberlist/restart) { get; set; } | Hämtar eller ställer in det numeriska värdet som åsidosätter det automatiska siffervärdet för listobjektet. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals#equals)(NumberList) | Bestämmer om det angivna objektet är lika med det aktuella objektet. |
| override [Equals](../../aspose.note/numberlist/equals#equals_1)(object) | Bestämmer om det angivna objektet är lika med det aktuella objektet. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode)() | Fungerar som en hashfunktion för typen. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader)(int) | Hämtar den numrerade listhuvudet. |

### Exempel

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

* namnutrymme [Aspose.Note](../../aspose.note)
* hopsättning [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
