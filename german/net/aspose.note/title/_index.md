---
title: Title
second_title: Aspose.Note für .NET-API-Referenz
description: steht für einen Titel.
type: docs
weight: 950
url: /de/net/aspose.note/title/
---
## Title class

steht für einen Titel.

```csharp
public sealed class Title : CompositeNodeBase, ICompositeNode<RichText>, IPageChildNode
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Title](title#constructor)() | Initialisiert eine neue Instanz von[`Title`](../title) Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Document](../../aspose.note/node/document) { get; } | Ruft das Dokument des Knotens ab. |
| [HorizontalOffset](../../aspose.note/title/horizontaloffset) { get; set; } | Ruft den horizontalen Versatz ab oder legt ihn fest. |
| override [IsComposite](../../aspose.note/title/iscomposite) { get; } | Ruft einen Wert ab, der angibt, ob dieser Knoten zusammengesetzt ist. Wenn wahr, kann der Knoten untergeordnete Knoten haben. |
| [LastModifiedTime](../../aspose.note/title/lastmodifiedtime) { get; set; } | Ruft die letzte Änderungszeit ab oder setzt sie. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Ruft den nächsten Knoten auf derselben Knotenbaumebene ab. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Ruft den Knotentyp ab. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Ruft den übergeordneten Knoten ab. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Ruft den vorherigen Knoten auf derselben Knotenbaumebene ab. |
| [TitleDate](../../aspose.note/title/titledate) { get; set; } | Ruft eine Zeichenfolgendarstellung des Datums im Titel ab oder legt diese fest. |
| [TitleText](../../aspose.note/title/titletext) { get; set; } | Liest oder setzt den Text des Titels. |
| [TitleTime](../../aspose.note/title/titletime) { get; set; } | Ruft eine Zeichenfolgendarstellung der Uhrzeit im Titel ab oder legt sie fest. |
| [VerticalOffset](../../aspose.note/title/verticaloffset) { get; set; } | Ruft den vertikalen Offset ab oder legt ihn fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Accept](../../aspose.note/title/accept)(DocumentVisitor) | Akzeptiert den Besucher des Knotens. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/title/getchildnodes#getchildnodes_1)() | Alle untergeordneten Knoten nach Knotentyp abrufen. |
| [GetEnumerator](../../aspose.note/title/getenumerator)() | Gibt einen Enumerator zurück, der die untergeordneten Knoten von iteriert[`Title`](../title) . |

### Beispiele

Zeigt, wie der Seitenverlauf bearbeitet wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden und erstes untergeordnetes Element abrufen           
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

Zeigt, wie Sie einen Titel für eine Seite festlegen.

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

Zeigt, wie Sie ein Dokument erstellen und es mit Standardoptionen im HTML-Format speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote-Dokument initialisieren
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Im HTML-Format speichern
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Zeigt, wie man ein Dokument erstellt und einen bestimmten Seitenbereich im HTML-Format speichert.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote-Dokument initialisieren
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Im HTML-Format speichern
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Zeigt, wie ein Dokument mit Titelseite erstellt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Aspose.Note.Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Eigenschaften des Seitentitels festlegen
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Seitenknoten im Dokument anhängen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Zeigt, wie ein Dokument in verschiedenen Formaten gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Das neue Dokument initialisieren
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Neue Seite initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Seitenknoten anhängen
doc.AppendChildLast(page);

// OneNote-Dokument in verschiedenen Formaten speichern, Textschriftgröße festlegen und Layoutänderungen manuell erkennen.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Siehe auch

* class [CompositeNodeBase](../compositenodebase)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1)
* class [RichText](../richtext)
* interface [IPageChildNode](../ipagechildnode)
* namensraum [Aspose.Note](../../aspose.note)
* Montage [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
