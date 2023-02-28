---
title: Image.Tags
second_title: Aspose.Note för .NET API-referens
description: Image fast egendom. Hämtar listan över alla taggar i ett stycke.
type: docs
weight: 160
url: /sv/net/aspose.note/image/tags/
---
## Image.Tags property

Hämtar listan över alla taggar i ett stycke.

```csharp
public List<ITag> Tags { get; }
```

### Exempel

Visar hur man lägger till ny bild med tagg.

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

// Ladda en bild
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Infoga bild i dokumentnoden
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Lägg till nod för dispositionselement
outline.AppendChildLast(outlineElem);

// Lägg till dispositionsnod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### Se även

* interface [ITag](../../itag/)
* class [Image](../)
* namnutrymme [Aspose.Note](../../image/)
* hopsättning [Aspose.Note](../../../)


