---
title: Image.Width
second_title: Aspose.Note voor .NET API-referentie
description: Image eigendom. Haalt of stelt de breedte in. Dit is de werkelijke breedte van de afbeelding in het MS OneNotedocument.
type: docs
weight: 180
url: /nl/net/aspose.note/image/width/
---
## Image.Width property

Haalt of stelt de breedte in. Dit is de werkelijke breedte van de afbeelding in het MS OneNote-document.

```csharp
public float Width { get; set; }
```

### Voorbeelden

Laat zien hoe u de meta-informatie van de afbeelding kunt krijgen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Haal alle afbeeldingsknooppunten op
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


