---
title: RichText.Text
second_title: Aspose.Note voor .NET API-referentie
description: RichText eigendom. Haalt of stelt de tekst in. De tekenreeks MAG GEEN tekens met de waarde 10 line feed bevatten.
type: docs
weight: 100
url: /nl/net/aspose.note/richtext/text/
---
## RichText.Text property

Haalt of stelt de tekst in. De tekenreeks MAG GEEN tekens met de waarde 10 (line feed) bevatten.

```csharp
public string Text { get; set; }
```

### Voorbeelden

Laat zien hoe u alle tekst uit het document kunt halen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Tekst ophalen
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Print tekst op het uitvoerscherm
Console.WriteLine(text);
```

Laat zien hoe u alle tekst van de pagina kunt halen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Krijg een lijst met paginaknooppunten
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Tekst ophalen
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Print tekst op het uitvoerscherm
    Console.WriteLine(text);
}
```

Laat zien hoe u tekst kunt ophalen uit de rij van elke tabel.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tables();

// Laad het document in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Krijg een lijst met tabelknooppunten
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Doorloop tabelrijen
    foreach (TableRow row in table)
    {
        // Tekst ophalen
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Print tekst op het uitvoerscherm
        Console.WriteLine(text);
    }
}
```

Laat zien hoe je tekst uit een tabel haalt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tables();

// Laad het document in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Krijg een lijst met tabelknooppunten
IList<Table> nodes = document.GetChildNodes<Table>();

// Stel het aantal tafels in
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Tekst ophalen
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Print tekst op het uitvoerscherm
    Console.WriteLine(text);
}
```

Laat zien hoe u een titel voor een pagina instelt.

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

Laat zien hoe u alle pagina's kunt doorlopen en een vervanging in de tekst kunt maken.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle RichText-knooppunten op
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Vervang tekst van een vorm
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Sla op in elk ondersteund bestandsformaat
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Laat zien hoe tekst uit de cellen van een tabel kan worden gehaald.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tables();

// Laad het document in Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Krijg een lijst met tabelknooppunten
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Doorloop tabelrijen
    foreach (TableRow row in table)
    {
        // Krijg een lijst met TableCell-knooppunten
        // Doorloop tabelcellen
        foreach (TableCell cell in row)
        {
            // Tekst ophalen
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Print tekst op het uitvoerscherm
            Console.WriteLine(text);
        }
    }
}
```

Laat zien hoe u een document maakt en opslaat in html-indeling met standaardopties.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiseer OneNote-document
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Opslaan in HTML-formaat
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Laat zien hoe je een nieuwe paragraaf met tag kunt toevoegen.

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
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// Tekstknooppunt toevoegen
outlineElem.AppendChildLast(text);

// Voeg overzichtselementknooppunt toe
outline.AppendChildLast(outlineElem);

// Voeg overzichtsknooppunt toe
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een document maakt en opslaat in een opgegeven paginabereik in html-indeling.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiseer OneNote-document
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Opslaan in HTML-formaat
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Laat zien hoe u toegang krijgt tot de details van een tag.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Haal alle RichText-knooppunten op
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Doorloop elk knooppunt
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Eigenschappen ophalen
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

Laat zien hoe je een document maakt met een tekst.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Page page = new Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Initialiseer het klasseobject TextStyle en stel opmaakeigenschappen in
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialiseer het RichText-klasseobject en pas tekststijl toe
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// RichText-knooppunt toevoegen
outlineElem.AppendChildLast(text);

// Voeg een OutlineElement-knooppunt toe
outline.AppendChildLast(outlineElem);

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
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

Laat zien hoe je een nieuwe lijst met opsommingstekens invoegt.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Maak een object van de klasse Document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klassenobject
Outline outline = new Outline(doc);

// Initialiseer het klasseobject TextStyle en stel opmaakeigenschappen in
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialiseer de klasse-objecten van OutlineElement en pas opsommingstekens toe
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Initialiseer het RichText-klasseobject en pas tekststijl toe
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
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
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
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

Laat zien hoe u een sjabloon voorbereidt voor een wekelijkse vergadering.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Maak een object van de klasse Document
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

Laat zien hoe u een hyperlink aan een tekst koppelt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tasks();

// Maak een object van de klasse Document
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

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem);

// Initialiseer het titelklasse-object
Title title = new Title() { TitleText = titleText };

// Initialiseer het paginaklasse-object
Page page = new Note.Page() { Title = title };

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Zie ook

* class [RichText](../)
* naamruimte [Aspose.Note](../../richtext/)
* montage [Aspose.Note](../../../)


