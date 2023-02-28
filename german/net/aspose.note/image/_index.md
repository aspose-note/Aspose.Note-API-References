---
title: Class Image
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Image klas. steht für ein Bild.
type: docs
weight: 250
url: /de/net/aspose.note/image/
---
## Image class

steht für ein Bild.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Image](image/#constructor)() | Initialisiert eine neue Instanz von`Image` Klasse. |
| [Image](image/#constructor_4)(string, Stream) | Initialisiert eine neue Instanz von`Image` Klasse. |
| [Image](image/#constructor_5)(string, string, string) | Initialisiert eine neue Instanz von`Image` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | Ruft die Ausrichtung ab oder legt sie fest. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | Holt oder setzt einen Body oder alternativen Text für das Bild. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | Ruft einen alternativen Texttitel für das Bild ab oder legt ihn fest. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | Ruft den Bilddatenspeicher ab. |
| [Document](../../aspose.note/node/document/) { get; } | Ruft das Dokument des Knotens ab. |
| [FileName](../../aspose.note/image/filename/) { get; } | Ruft den Dateinamen ab. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | Ruft den Pfad zur Bilddatei ab. |
| [Format](../../aspose.note/image/format/) { get; } | Ruft das Format des Bildes ab. |
| [Height](../../aspose.note/image/height/) { get; set; } | Holt oder setzt die Höhe. Dies ist die tatsächliche Höhe des Bildes im MS OneNote-Dokument. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | Ruft den horizontalen Versatz ab oder legt ihn fest. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | Ruft den dem Bild zugeordneten Hyperlink ab oder legt ihn fest. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | Ruft ab, ob das Bild ein Hintergrundbild ist. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Ruft einen Wert ab, der angibt, ob dieser Knoten zusammengesetzt ist. Wenn wahr, kann der Knoten untergeordnete Knoten haben. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | Ruft die letzte Änderungszeit ab oder legt sie fest. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Ruft den nächsten Knoten auf derselben Knotenbaumebene ab. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Ruft den Knotentyp ab. |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | Ruft die ursprüngliche Höhe ab. Dies ist die ursprüngliche Breite des Bildes vor der Größenänderung. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | Ruft die ursprüngliche Breite ab. Dies ist die ursprüngliche Breite des Bildes vor der Größenänderung. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Ruft den übergeordneten Knoten ab. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Ruft den vorherigen Knoten auf derselben Knotenbaumebene ab. |
| [Tags](../../aspose.note/image/tags/) { get; } | Ruft die Liste aller Tags eines Absatzes ab. |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | Ruft den vertikalen Offset ab oder legt ihn fest. |
| [Width](../../aspose.note/image/width/) { get; set; } | Holt oder setzt die Breite. Dies ist die tatsächliche Breite des Bilds im MS OneNote-Dokument. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | Akzeptiert den Besucher des Knotens. |

### Beispiele

Zeigt, wie ein Hyperlink an ein Bild gebunden wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Zeigt, wie eine Textbeschreibung für ein Bild festgelegt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

Zeigt, wie ein Bild aus einem Dokument abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Alle Image-Knoten abrufen
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Bildbytes in einer Datei speichern
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Zeigt, wie die Metainformationen des Bildes abgerufen werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Alle Image-Knoten abrufen
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

Zeigt, wie ein Bild aus einer Datei zu einem Dokument mit benutzerdefinierten Eigenschaften hinzugefügt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Dokument aus dem Stream laden.
Document doc = new Document(dataDir + "Aspose.one");

// Holen Sie sich die erste Seite des Dokuments.
Aspose.Note.Page page = doc.FirstChild;

// Laden Sie ein Bild aus der Datei.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ändern Sie die Größe des Bildes nach Ihren Bedürfnissen (optional).
                              Width = 100,
                              Height = 100,

                              // Legen Sie die Position des Bildes auf der Seite fest (optional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Bildausrichtung festlegen
                              Alignment = HorizontalAlignment.Right
                          };

// Bild zur Seite hinzufügen.
page.AppendChildLast(image);
```

Zeigt, wie ein Bild aus einem Stream zu einem Dokument hinzugefügt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Laden Sie das zweite Bild unter Verwendung des Bildnamens, der Erweiterung und des Streams.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Bildausrichtung festlegen
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Zeigt, wie Sie einem Dokument ein Bild aus einer Datei hinzufügen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren und Offset-Eigenschaften festlegen
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

// Laden Sie ein Bild über den Dateipfad.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Bildausrichtung festlegen
                              Alignment = HorizontalAlignment.Right
                          };

// Bild hinzufügen
outlineElem.AppendChildLast(image);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Siehe auch

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


