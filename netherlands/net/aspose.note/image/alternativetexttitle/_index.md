---
title: Image.AlternativeTextTitle
second_title: Aspose.Note voor .NET API-referentie
description: Image eigendom. Haalt of stelt een titel van alternatieve tekst voor de afbeelding in.
type: docs
weight: 40
url: /nl/net/aspose.note/image/alternativetexttitle/
---
## Image.AlternativeTextTitle property

Haalt of stelt een titel van alternatieve tekst voor de afbeelding in.

```csharp
public string AlternativeTextTitle { get; set; }
```

### Voorbeelden

Laat zien hoe u een tekstbeschrijving voor een afbeelding instelt.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* class [Image](../)
* naamruimte [Aspose.Note](../../image/)
* montage [Aspose.Note](../../../)


