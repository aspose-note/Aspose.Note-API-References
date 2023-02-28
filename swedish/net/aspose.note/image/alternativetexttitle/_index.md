---
title: Image.AlternativeTextTitle
second_title: Aspose.Note för .NET API-referens
description: Image fast egendom. Hämtar eller ställer in en titel på alternativ text för bilden.
type: docs
weight: 40
url: /sv/net/aspose.note/image/alternativetexttitle/
---
## Image.AlternativeTextTitle property

Hämtar eller ställer in en titel på alternativ text för bilden.

```csharp
public string AlternativeTextTitle { get; set; }
```

### Exempel

Visar hur man ställer in textbeskrivning för en bild.

```csharp
// Sökvägen till dokumentkatalogen.
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

### Se även

* class [Image](../)
* namnutrymme [Aspose.Note](../../image/)
* hopsättning [Aspose.Note](../../../)


