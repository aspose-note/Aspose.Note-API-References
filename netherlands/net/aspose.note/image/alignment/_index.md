---
title: Image.Alignment
second_title: Aspose.Note voor .NET API-referentie
description: Image eigendom. Haalt of stelt de uitlijning in.
type: docs
weight: 20
url: /nl/net/aspose.note/image/alignment/
---
## Image.Alignment property

Haalt of stelt de uitlijning in.

```csharp
public HorizontalAlignment Alignment { get; set; }
```

### Voorbeelden

Laat zien hoe u een afbeelding uit een bestand toevoegt aan een document met door de gebruiker gedefinieerde eigenschappen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad document uit de stream.
Document doc = new Document(dataDir + "Aspose.one");

// Haal de eerste pagina van het document op.
Aspose.Note.Page page = doc.FirstChild;

// Laad een afbeelding uit het bestand.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Wijzig de grootte van de afbeelding volgens uw behoeften (optioneel).
                              Width = 100,
                              Height = 100,

                              // Stel de locatie van de afbeelding op de pagina in (optioneel).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Beelduitlijning instellen
                              Alignment = HorizontalAlignment.Right
                          };

// Voeg de afbeelding toe aan de pagina.
page.AppendChildLast(image);
```

Laat zien hoe u een afbeelding uit een stream toevoegt aan een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Laad de tweede afbeelding met de afbeeldingsnaam, extensie en stream.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Beelduitlijning instellen
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Laat zien hoe u een afbeelding uit een bestand toevoegt aan een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het paginaklasse-object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialiseer het Outline-klasseobject en stel offset-eigenschappen in
Outline outline = new Outline(doc);

// Initialiseer het klasseobject OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Laad een afbeelding via het bestandspad.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Beelduitlijning instellen
                              Alignment = HorizontalAlignment.Right
                          };

// Voeg afbeelding toe
outlineElem.AppendChildLast(image);

// Voeg overzichtselementen toe
outline.AppendChildLast(outlineElem);

// Overzichtsknooppunt toevoegen
page.AppendChildLast(outline);

// Paginaknooppunt toevoegen
doc.AppendChildLast(page);

// Sla OneNote-document op
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Zie ook

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* naamruimte [Aspose.Note](../../image/)
* montage [Aspose.Note](../../../)


