---
title: Class Page
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Page klas. Vertegenwoordigt een pagina.
type: docs
weight: 480
url: /nl/net/aspose.note/page/
---
## Page class

Vertegenwoordigt een pagina.

```csharp
public sealed class Page : CompositeNode<IPageChildNode>
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Page](page/#constructor)() | Initialiseert een nieuw exemplaar van het`Page` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Author](../../aspose.note/page/author/) { get; set; } | Haalt of stelt de auteur in. |
| [BackgroundColor](../../aspose.note/page/backgroundcolor/) { get; set; } | Hiermee wordt de achtergrondkleur van de pagina opgehaald of ingesteld. |
| [CreationTime](../../aspose.note/page/creationtime/) { get; set; } | Haalt of stelt de aanmaaktijd in. |
| [Document](../../aspose.note/node/document/) { get; } | Haalt het document van het knooppunt op. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [IsConflictPage](../../aspose.note/page/isconflictpage/) { get; set; } | Haalt of stelt een waarde in die aangeeft of deze pagina een conflictpagina is. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/page/lastmodifiedtime/) { get; set; } | Haalt of stelt de laatst gewijzigde tijd in. |
| [Level](../../aspose.note/page/level/) { get; set; } | Haalt of stelt het niveau in. |
| [Margin](../../aspose.note/page/margin/) { get; set; } | Haalt of stelt de marge in. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Haalt het volgende knooppunt op op hetzelfde knooppuntboomniveau. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Haalt het knooppunttype op. |
| [PageContentRevisionSummary](../../aspose.note/page/pagecontentrevisionsummary/) { get; set; } | Haalt of stelt het revisieoverzicht voor de pagina en de onderliggende knooppunten in. |
| [PageLayoutSize](../../aspose.note/page/pagelayoutsize/) { get; set; } | Hiermee wordt de lay-outgrootte van de pagina weergegeven in de editor opgehaald of ingesteld. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Haalt het bovenliggende knooppunt op. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Haalt het vorige knooppunt op hetzelfde knooppuntboomniveau. |
| [SizeType](../../aspose.note/page/sizetype/) { get; set; } | Hiermee wordt het formaattype van een pagina opgehaald of ingesteld. |
| [Title](../../aspose.note/page/title/) { get; set; } | Haalt of stelt de titel in. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [Accept](../../aspose.note/page/accept/)(DocumentVisitor) | Accepteert de bezoeker van de node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [Clone](../../aspose.note/page/clone/)(bool) | Kloont de pagina. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/page/getchildnodes/#getchildnodes_1)() | Alle onderliggende knooppunten van de pagina ophalen op basis van het knooppunttype. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IPageChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IPageChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Voorbeelden

Laat zien hoe u de achtergrondkleur van de pagina instelt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

Laat zien hoe u meta-informatie over een pagina kunt krijgen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
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

Laat zien hoe u de geschiedenis van de pagina kunt ophalen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad OneNote-document
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Haal de eerste pagina op
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

Laat zien hoe u de meta-informatie van de pagina kunt bewerken.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Samenvatting inhoudsrevisie voor deze pagina lezen
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Werk de samenvatting van de paginarevisie bij voor deze pagina
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
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

Laat zien hoe u door de tekst van de pagina kunt gaan en een vervanging kunt maken.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Haal alle RichText-knooppunten op
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Vervang tekst van een vorm
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Sla op in elk ondersteund bestandsformaat
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
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

Laat zien hoe u kunt controleren of een pagina een conflictpagina is (dwz dat deze wijzigingen bevat die OneNote niet automatisch kan samenvoegen).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Laad OneNote-document
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Standaard worden conflictpagina's gewoon overgeslagen bij het opslaan.
    // Als u het als niet-conflict markeert, wordt het zoals gebruikelijk in de geschiedenis opgeslagen.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
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

Laat zien hoe u een document met een titelpagina maakt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Maak een object van de klasse Document
Document doc = new Aspose.Note.Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Stel de eigenschappen van de paginatitel in
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Voeg een paginaknooppunt toe aan het document
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een document in verschillende indelingen kunt opslaan.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialiseer het nieuwe document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initialiseer de nieuwe pagina
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standaardstijl voor alle tekst in het document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Bewaar OneNote-document in verschillende formaten, stel de lettergrootte van tekst in en detecteer lay-outwijzigingen handmatig.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
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

Laat zien hoe u een pagina met een subpagina kunt toevoegen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het Page class-object en stel het niveau in
Aspose.Note.Page page1 = new Aspose.Note.Page(doc) { Level = 1 };

// Initialiseer het Page class-object en stel het niveau in
Aspose.Note.Page page2 = new Aspose.Note.Page(doc) { Level = 2 };

// Initialiseer het Page class-object en stel het niveau in
Aspose.Note.Page page3 = new Aspose.Note.Page(doc) { Level = 1 };

/*---------- Adding nodes to first Page ----------*/
Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "First page.", ParagraphStyle = textStyle };
outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page1.AppendChildLast(outline);

/*---------- Adding nodes to second Page ----------*/
var outline2 = new Outline(doc);
var outlineElem2 = new OutlineElement(doc);
var textStyle2 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text2 = new RichText(doc) { Text = "Second page.", ParagraphStyle = textStyle2 };
outlineElem2.AppendChildLast(text2);
outline2.AppendChildLast(outlineElem2);
page2.AppendChildLast(outline2);

/*---------- Adding nodes to third Page ----------*/
var outline3 = new Outline(doc);
var outlineElem3 = new OutlineElement(doc);
var textStyle3 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text3 = new RichText(doc) { Text = "Third page.", ParagraphStyle = textStyle3 };
outlineElem3.AppendChildLast(text3);
outline3.AppendChildLast(outlineElem3);
page3.AppendChildLast(outline3);

/*---------- Add pages to the OneNote Document ----------*/
doc.AppendChildLast(page1);
doc.AppendChildLast(page2);
doc.AppendChildLast(page3);

// Sla OneNote-document op
dataDir = dataDir + "CreateDocWithRootAndSubPages_out.one";
doc.Save(dataDir);
```

### Zie ook

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IPageChildNode](../ipagechildnode/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


