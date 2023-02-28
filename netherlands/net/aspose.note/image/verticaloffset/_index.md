---
title: Image.VerticalOffset
second_title: Aspose.Note voor .NET API-referentie
description: Image eigendom. Haalt of stelt de verticale offset in.
type: docs
weight: 170
url: /nl/net/aspose.note/image/verticaloffset/
---
## Image.VerticalOffset property

Haalt of stelt de verticale offset in.

```csharp
public float VerticalOffset { get; set; }
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

### Zie ook

* class [Image](../)
* naamruimte [Aspose.Note](../../image/)
* montage [Aspose.Note](../../../)


