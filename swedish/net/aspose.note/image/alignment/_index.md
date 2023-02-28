---
title: Image.Alignment
second_title: Aspose.Note för .NET API-referens
description: Image fast egendom. Hämtar eller ställer in justeringen.
type: docs
weight: 20
url: /sv/net/aspose.note/image/alignment/
---
## Image.Alignment property

Hämtar eller ställer in justeringen.

```csharp
public HorizontalAlignment Alignment { get; set; }
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

Visar hur man lägger till en bild från ström till ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Ladda den andra bilden med bildnamnet, tillägget och strömmen.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Ställ in bildjustering
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Visar hur man lägger till en bild från fil till ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Images();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initiera Outline-klassobjektet och ställ in offsetegenskaper
Outline outline = new Outline(doc);

// Initiera OutlineElement-klassobjekt
OutlineElement outlineElem = new OutlineElement(doc);

// Ladda en bild efter filsökvägen.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ställ in bildjustering
                              Alignment = HorizontalAlignment.Right
                          };

// Lägg till bild
outlineElem.AppendChildLast(image);

// Lägg till konturelement
outline.AppendChildLast(outlineElem);

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Se även

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* namnutrymme [Aspose.Note](../../image/)
* hopsättning [Aspose.Note](../../../)


