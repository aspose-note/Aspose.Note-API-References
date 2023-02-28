---
title: Class Title
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Title klas. Vertegenwoordigt een titel.
type: docs
weight: 980
url: /nl/net/aspose.note/title/
---
## Title class

Vertegenwoordigt een titel.

```csharp
public sealed class Title : CompositeNodeBase, ICompositeNode<RichText>, IPageChildNode
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Title](title/#constructor)() | Initialiseert een nieuw exemplaar van het`Title` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Haalt het document van het knooppunt op. |
| [HorizontalOffset](../../aspose.note/title/horizontaloffset/) { get; set; } | Haalt of stelt de horizontale offset in. |
| override [IsComposite](../../aspose.note/title/iscomposite/) { get; } | Krijgt een waarde die aangeeft of dit knooppunt samengesteld is. Indien waar, kan het knooppunt onderliggende knooppunten hebben. |
| [LastModifiedTime](../../aspose.note/title/lastmodifiedtime/) { get; set; } | Haalt of stelt de laatst gewijzigde tijd in. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Haalt het volgende knooppunt op op hetzelfde knooppuntboomniveau. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Haalt het knooppunttype op. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Haalt het bovenliggende knooppunt op. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Haalt het vorige knooppunt op hetzelfde knooppuntboomniveau. |
| [TitleDate](../../aspose.note/title/titledate/) { get; set; } | Haalt of stelt een tekenreeksvoorstelling van de datum in de titel in. |
| [TitleText](../../aspose.note/title/titletext/) { get; set; } | Haalt of stelt de tekst van de titel in. |
| [TitleTime](../../aspose.note/title/titletime/) { get; set; } | Haalt of stelt een tekenreeksrepresentatie in van de tijd in de titel. |
| [VerticalOffset](../../aspose.note/title/verticaloffset/) { get; set; } | Haalt of stelt de verticale offset in. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [Accept](../../aspose.note/title/accept/)(DocumentVisitor) | Accepteert de bezoeker van de node. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/title/getchildnodes/#getchildnodes_1)() | Alle onderliggende knooppunten ophalen op basis van het knooppunttype. |
| [GetEnumerator](../../aspose.note/title/getenumerator/)() | Retourneert een teller die itereert door onderliggende knooppunten van het`Title` . |

### Voorbeelden

Laat zien hoe u de geschiedenis van de pagina kunt bewerken.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
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

### Zie ook

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* class [RichText](../richtext/)
* interface [IPageChildNode](../ipagechildnode/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


