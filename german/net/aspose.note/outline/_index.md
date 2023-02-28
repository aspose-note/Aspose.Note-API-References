---
title: Class Outline
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Outline klas. steht für eine Gliederung.
type: docs
weight: 450
url: /de/net/aspose.note/outline/
---
## Outline class

steht für eine Gliederung.

```csharp
public sealed class Outline : IndentatedNode<IOutlineChildNode>, IPageChildNode
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Outline](outline/#constructor)() | Initialisiert eine neue Instanz von`Outline` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DescendantsCannotBeMoved](../../aspose.note/outline/descendantscannotbemoved/) { get; set; } | Ruft ab, ob Nachkommen der Gliederung verschoben werden können. |
| [Document](../../aspose.note/node/document/) { get; } | Ruft das Dokument des Knotens ab. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [HorizontalOffset](../../aspose.note/outline/horizontaloffset/) { get; set; } | Ruft den horizontalen Versatz ab oder legt ihn fest. |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/outline/lastmodifiedtime/) { get; set; } | Ruft die letzte Änderungszeit ab oder setzt sie. |
| [MaxHeight](../../aspose.note/outline/maxheight/) { get; set; } | Ruft die maximale Höhe ab oder legt sie fest. |
| [MaxWidth](../../aspose.note/outline/maxwidth/) { get; set; } | Ruft die maximale Breite ab oder legt sie fest. |
| [MinWidth](../../aspose.note/outline/minwidth/) { get; set; } | Ruft die Mindestbreite ab oder legt sie fest. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Ruft den nächsten Knoten auf derselben Knotenbaumebene ab. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Ruft den Knotentyp ab. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Ruft den übergeordneten Knoten ab. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Ruft den vorherigen Knoten auf derselben Knotenbaumebene ab. |
| [ReservedWidth](../../aspose.note/outline/reservedwidth/) { get; set; } | Ruft die reservierte Breite ab oder legt sie fest. |
| [VerticalOffset](../../aspose.note/outline/verticaloffset/) { get; set; } | Ruft den vertikalen Offset ab oder legt ihn fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Accept](../../aspose.note/outline/accept/)(DocumentVisitor) | Akzeptiert den Besucher des Knotens. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Beispiele

Zeigt, wie man ein neues Bild mit Tag hinzufügt.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

// Laden Sie ein Bild
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Bild in den Dokumentknoten einfügen
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Gliederungselementknoten hinzufügen
outline.AppendChildLast(outlineElem);

// Gliederungsknoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

Zeigt, wie eine neue Liste mit chinesischer Nummerierung eingefügt wird.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// OneNote-Dokument initialisieren
Aspose.Note.Document doc = new Aspose.Note.Document();

// OneNote-Seite initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Textstileinstellungen anwenden
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Zahlen in derselben Gliederung werden automatisch erhöht.
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

// OneNote-Dokument speichern
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Zeigt, wie neue Listen mit Aufzählungszeichen eingefügt werden.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Erstellen Sie ein Objekt der Document-Klasse
Aspose.Note.Document doc = new Aspose.Note.Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// TextStyle-Klassenobjekt initialisieren und Formatierungseigenschaften festlegen
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Objekte der OutlineElement-Klasse initialisieren und Aufzählungszeichen anwenden
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// RichText-Klassenobjekt initialisieren und Textstil anwenden
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);
// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Zeigt, wie eine neue Liste mit Nummerierung eingefügt wird.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// TextStyle-Klassenobjekt initialisieren und Formatierungseigenschaften festlegen
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Objekte der OutlineElement-Klasse initialisieren und Nummerierung anwenden
// Zahlen in derselben Gliederung werden automatisch erhöht.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Siehe auch

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


