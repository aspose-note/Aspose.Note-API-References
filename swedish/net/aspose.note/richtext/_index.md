---
title: Class RichText
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.RichText klass. Representerar en rik text.
type: docs
weight: 530
url: /sv/net/aspose.note/richtext/
---
## RichText class

Representerar en rik text.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [RichText](richtext/#constructor)() | Initierar en ny instans av`RichText` class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | Hämtar eller ställer in justeringen. |
| [Document](../../aspose.note/node/document/) { get; } | Hämtar dokumentet för noden. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Får ett värde som indikerar om denna nod är sammansatt. Om sant kan noden ha underordnade noder. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | Hämtar eller ställer in den senast ändrade tiden. |
| [Length](../../aspose.note/richtext/length/) { get; } | Får längden på texten. |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | Hämtar eller ställer in radavståndet. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Hämtar nodtypen. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | Hämtar eller ställer in styckeformatet. Dessa inställningar används om det inte finns något matchande TextStyle-objekt iStyles samling antingen anger detta objekt inte en nödvändig inställning. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Hämtar föregående nod på samma nodträdsnivå. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | Hämtar eller ställer in minsta möjliga utrymme efter. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | Hämtar eller ställer in minsta möjliga utrymme innan. |
| [Tags](../../aspose.note/richtext/tags/) { get; } | Hämtar listan över alla taggar i ett stycke. |
| [Text](../../aspose.note/richtext/text/) { get; set; } | Hämtar eller ställer in texten. Strängen FÅR INTE innehålla några tecken med värdet 10 (radmatning). |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | Hämtar samlingen av textkörningar. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | Accepterar besökaren av noden. |
| [Append](../../aspose.note/richtext/append/#append)(string) | Lägger till en sträng till det sista textintervallet. |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | Lägger till en sträng i slutet. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | Lägger till en sträng längst fram i det första textintervallet. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | Lägger till en sträng på framsidan. |
| [Clear](../../aspose.note/richtext/clear/)() | Rensar innehållet i denna instans. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | Returnerar en uppräkning som itererar genom tecken i detta RichText-objekt. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | Returnerar det nollbaserade indexet för den första förekomsten av det angivna Unicode-tecknet i denna sträng. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i denna instans. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | Returnerar det nollbaserade indexet för den första förekomsten av det angivna Unicode-tecknet i denna sträng. Sökningen startar vid en angiven teckenposition. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i det här fallet. Sökningen startar vid en angiven teckenposition. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i den aktuella instansen. En parameter anger vilken typ av sökning som ska användas för den angivna strängen. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | Returnerar det nollbaserade indexet för den första förekomsten av det angivna tecknet i den här instansen. Sökningen startar vid en angiven teckenposition och undersöker ett specificerat antal teckenpositioner. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i det här fallet. Sökningen startar vid en angiven teckenposition och undersöker ett specificerat antal teckenpositioner. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i den aktuella instansen. Parametrar anger startsökningspositionen i den aktuella strängen och vilken typ av sökning som ska användas för den angivna strängen. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | Returnerar det nollbaserade indexet för den första förekomsten av den angivna strängen i den aktuella instansen. |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | Infogar en specificerad sträng vid en angiven indexposition i den här instansen. |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | Infogar en specificerad sträng med specificerad stil vid en angiven indexposition i denna instans. |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | Tar bort alla tecken i den aktuella instansen, börjar på en angiven position och fortsätter genom den sista positionen. |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | Tar bort specificerat antal tecken i den aktuella instansen som börjar på en angiven position. |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | Ersätter alla förekomster av ett specificerat Unicode-tecken i det här fallet med ett annat specificerat Unicode-tecken. |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | Ersätter alla förekomster av en angiven sträng i den aktuella instansen med en annan specificerad sträng. |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | Ersätter alla förekomster av en angiven sträng i den aktuella instansen med en annan specificerad sträng i angiven stil. |
| [Trim](../../aspose.note/richtext/trim/#trim)() | Tar bort alla inledande och efterföljande blanktecken. |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | Tar bort alla inledande och efterföljande förekomster av en karaktär. |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | Tar bort alla inledande och efterföljande förekomster av en uppsättning tecken som anges i en array. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | Tar bort alla efterföljande blanktecken. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | Tar bort alla efterföljande förekomster av en karaktär. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | Tar bort alla efterföljande förekomster av en uppsättning tecken som anges i en array. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | Tar bort alla inledande blanktecken. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | Tar bort alla inledande förekomster av ett angivet tecken. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | Tar bort alla inledande förekomster av en uppsättning tecken som anges i en array. |

### Exempel

Visar hur man hämtar all text från dokumentet.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta text
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Skriv ut text på utdataskärmen
Console.WriteLine(text);
```

Visar hur man hämtar all text från sidan.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Få lista över sidnoder
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Hämta text
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Skriv ut text på utdataskärmen
    Console.WriteLine(text);
}
```

Låt oss betona sidans titlar bland andra rubriker genom att öka teckensnittets storlek.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Iterera genom sidans titlar.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

Visar hur man hämtar text från varje tabells rad.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tables();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Få en lista över tabellnoder
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Iterera genom tabellrader
    foreach (TableRow row in table)
    {
        // Hämta text
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Skriv ut text på utdataskärmen
        Console.WriteLine(text);
    }
}
```

Visar hur man hämtar text från en tabell.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tables();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Få en lista över tabellnoder
IList<Table> nodes = document.GetChildNodes<Table>();

// Ange tabellräkning
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Hämta text
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Skriv ut text på utdataskärmen
    Console.WriteLine(text);
}
```

Låt oss betona de senaste textens ändringar genom att markera.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Få RichText-noder modifierade förra veckan.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Ställ in högdagerfärg
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Ställ in högdagerfärg
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
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

Ställ in korrekturspråk för en text.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

Visar hur man går igenom alla sidor och gör en ersättning i texten.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Hämta alla RichText-noder
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Ersätt text i en form
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Spara till valfritt filformat som stöds
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Manipulera efter textformat med hjälp av styckeformat.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

Visar hur man hämtar text från en tabells celler.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tables();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Få en lista över tabellnoder
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Iterera genom tabellrader
    foreach (TableRow row in table)
    {
        // Få lista över TableCell-noder
        // Iterera genom tabellceller
        foreach (TableCell cell in row)
        {
            // Hämta text
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Skriv ut text på utdataskärmen
            Console.WriteLine(text);
        }
    }
}
```

Visar hur man går igenom sidans text och gör en ersättning.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Hämta alla RichText-noder
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Ersätt text i en form
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Spara till valfritt filformat som stöds
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
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

Visar hur man lägger till ett nytt stycke med tagg.

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
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// Lägg till textnod
outlineElem.AppendChildLast(text);

// Lägg till nod för dispositionselement
outline.AppendChildLast(outlineElem);

// Lägg till dispositionsnod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "AddTextNodeWithTag_out.one";
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

Visar hur du kommer åt information om en tagg.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tags();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Hämta alla RichText-noder
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterera genom varje nod
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Hämta egenskaper
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

Visar hur man skapar ett dokument med en text.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Page page = new Page(doc);

// Initiera Outline-klassobjekt
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

// Initiera TextStyle-klassobjektet och ställ in formateringsegenskaper
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initiera RichText-klassobjekt och tillämpa textstil
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// Lägg till RichText-nod
outlineElem.AppendChildLast(text);

// Lägg till OutlineElement-nod
outline.AppendChildLast(outlineElem);

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
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

Visar hur man förbereder en mall för veckomöte.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tags();

// Skapa ett objekt av klassen Document
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
```

Visar hur man binder en hyperlänk till en text.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Tasks();

// Skapa ett objekt av klassen Document
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Lägg till konturelement
outline.AppendChildLast(outlineElem);

// Initiera Title-klassobjekt
Title title = new Title() { TitleText = titleText };

// Initiera Sidklassobjekt
Page page = new Note.Page() { Title = title };

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Se även

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


