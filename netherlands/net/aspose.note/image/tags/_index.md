---
title: Image.Tags
second_title: Aspose.Note voor .NET API-referentie
description: Image eigendom. Krijgt de lijst met alle tags van een paragraaf.
type: docs
weight: 160
url: /nl/net/aspose.note/image/tags/
---
## Image.Tags property

Krijgt de lijst met alle tags van een paragraaf.

```csharp
public List<ITag> Tags { get; }
```

### Voorbeelden

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

### Zie ook

* interface [ITag](../../itag/)
* class [Image](../)
* naamruimte [Aspose.Note](../../image/)
* montage [Aspose.Note](../../../)


