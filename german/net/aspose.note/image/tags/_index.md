---
title: Image.Tags
second_title: Aspose.Note für .NET-API-Referenz
description: Image eigendom. Ruft die Liste aller Tags eines Absatzes ab.
type: docs
weight: 160
url: /de/net/aspose.note/image/tags/
---
## Image.Tags property

Ruft die Liste aller Tags eines Absatzes ab.

```csharp
public List<ITag> Tags { get; }
```

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

### Siehe auch

* interface [ITag](../../itag/)
* class [Image](../)
* namensraum [Aspose.Note](../../image/)
* Montage [Aspose.Note](../../../)


