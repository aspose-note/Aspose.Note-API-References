---
title: AttachedFile
second_title: Aspose.Note für .NET-API-Referenz
description: Stellt eine angehängte Datei dar.
type: docs
weight: 10
url: /de/net/aspose.note/attachedfile/
---
## AttachedFile class

Stellt eine angehängte Datei dar.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [AttachedFile](attachedfile#constructor)() | Initialisiert eine neue Instanz von[`AttachedFile`](../attachedfile) Klasse. |
| [AttachedFile](attachedfile#constructor_6)(string, Stream) | Initialisiert eine neue Instanz von[`AttachedFile`](../attachedfile) Klasse. |
| [AttachedFile](attachedfile#constructor_7)(string, Stream, ImageFormat) | Initialisiert eine neue Instanz von[`AttachedFile`](../attachedfile) Klasse. |
| [AttachedFile](attachedfile#constructor_8)(string, Stream, Stream, ImageFormat) | Initialisiert eine neue Instanz von[`AttachedFile`](../attachedfile) Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment) { get; set; } | Ruft die Ausrichtung ab oder legt sie fest. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription) { get; set; } | Ruft einen alternativen Text für das Symbol der angehängten Datei ab oder legt ihn fest. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle) { get; set; } | Ruft einen alternativen Texttitel für das Symbol der angehängten Datei ab oder legt ihn fest. |
| [Bytes](../../aspose.note/attachedfile/bytes) { get; } | Ruft die Binärdaten für eine eingebettete Datei ab. |
| [Document](../../aspose.note/node/document) { get; } | Ruft das Dokument des Knotens ab. |
| [Extension](../../aspose.note/attachedfile/extension) { get; } | Ruft die Erweiterung einer eingebetteten Datei ab. |
| [FileName](../../aspose.note/attachedfile/filename) { get; } | Ruft den Namen der eingebetteten Datei ab. |
| [FilePath](../../aspose.note/attachedfile/filepath) { get; } | Ruft den Pfad zur Originaldatei ab. |
| [Height](../../aspose.note/attachedfile/height) { get; } | Ruft die ursprüngliche Höhe des eingebetteten Dateisymbols ab. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset) { get; set; } | Ruft den horizontalen Versatz ab oder legt ihn fest. |
| [Icon](../../aspose.note/attachedfile/icon) { get; } | Ruft die Binärdaten für das Symbol ab, das der eingebetteten Datei zugeordnet ist. |
| [IconExtension](../../aspose.note/attachedfile/iconextension) { get; } | Ruft die Erweiterung des Symbols ab. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Ruft einen Wert ab, der angibt, ob dieser Knoten zusammengesetzt ist. Wenn wahr, kann der Knoten untergeordnete Knoten haben. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Ansicht der Datei ein Ausdruck ist. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Wert der Größe des Symbols ausdrücklich vom Benutzer aktualisiert wurde. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime) { get; set; } | Ruft die letzte Änderungszeit ab oder setzt sie. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight) { get; set; } | Ruft die maximale Höhe zum Anzeigen des eingebetteten Dateisymbols ab oder legt sie fest. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth) { get; set; } | Ruft die maximale Breite zum Anzeigen des eingebetteten Dateisymbols ab oder legt sie fest. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Ruft den nächsten Knoten auf derselben Knotenbaumebene ab. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Ruft den Knotentyp ab. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Ruft den übergeordneten Knoten ab. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Ruft den vorherigen Knoten auf derselben Knotenbaumebene ab. |
| [Tags](../../aspose.note/attachedfile/tags) { get; } | Ruft die Liste aller Tags eines Absatzes ab. |
| [Text](../../aspose.note/attachedfile/text) { get; set; } | Ruft die Textdarstellung der eingebetteten Datei ab oder legt sie fest. Der String DARF KEINE Zeichen mit dem Wert 10 (Zeilenvorschub) oder 13 (Wagenrücklauf) enthalten. |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset) { get; set; } | Ruft den vertikalen Offset ab oder legt ihn fest. |
| [Width](../../aspose.note/attachedfile/width) { get; } | Ruft die ursprüngliche Breite des eingebetteten Dateisymbols ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept)(DocumentVisitor) | Akzeptiert den Besucher des Knotens. |

### Beispiele

Zeigt, wie der Inhalt einer angehängten Datei abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Attachments();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Holen Sie sich eine Liste der angehängten Dateiknoten
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Durch alle Knoten iterieren
foreach (AttachedFile file in nodes)
{
    // Angehängte Datei in ein Stream-Objekt laden
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Erstellen Sie eine lokale Datei
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Dateistrom kopieren
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Zeigt, wie Sie mithilfe von filepath eine Datei zu einem Dokument hinzufügen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Attachments();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

// AttachedFile-Klassenobjekt initialisieren
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Angehängte Datei hinzufügen
outlineElem.AppendChildLast(attachedFile);

// Gliederungselementknoten hinzufügen
outline.AppendChildLast(outlineElem);

// Gliederungsknoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Zeigt, wie eine Datei aus einem Stream zu einem Dokument hinzugefügt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Attachments();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Objekt der AttachedFile-Klasse initialisieren und auch seinen Icon-Pfad übergeben
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Angehängte Datei hinzufügen
    outlineElem.AppendChildLast(attachedFile);
}

// Gliederungselementknoten hinzufügen
outline.AppendChildLast(outlineElem);

// Gliederungsknoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### Siehe auch

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* namensraum [Aspose.Note](../../aspose.note)
* Montage [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
