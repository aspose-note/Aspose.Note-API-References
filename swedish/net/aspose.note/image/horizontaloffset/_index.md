---
title: Image.HorizontalOffset
second_title: Aspose.Note för .NET API-referens
description: Image fast egendom. Hämtar eller ställer in den horisontella offseten.
type: docs
weight: 100
url: /sv/net/aspose.note/image/horizontaloffset/
---
## Image.HorizontalOffset property

Hämtar eller ställer in den horisontella offseten.

```csharp
public float HorizontalOffset { get; set; }
```

### Exempel

Visar hur man lägger till en bild från fil till ett dokument med användardefinierade egenskaper.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Ladda dokument från strömmen.
Document doc = new Document(dataDir + "Aspose.one");

// Hämta den första sidan av dokumentet.
Aspose.Note.Page page = doc.FirstChild;

// Ladda en bild från filen.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ändra bildens storlek efter dina behov (valfritt).
                              Width = 100,
                              Height = 100,

                              // Ställ in bildens plats på sidan (valfritt).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Ställ in bildjustering
                              Alignment = HorizontalAlignment.Right
                          };

// Lägg till bilden på sidan.
page.AppendChildLast(image);
```

### Se även

* class [Image](../)
* namnutrymme [Aspose.Note](../../image/)
* hopsättning [Aspose.Note](../../../)


