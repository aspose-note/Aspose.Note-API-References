---
title: Image.HyperlinkUrl
second_title: Aspose.Note voor .NET API-referentie
description: Image eigendom. Haalt of stelt de hyperlink in die aan de afbeelding is gekoppeld.
type: docs
weight: 110
url: /nl/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

Haalt of stelt de hyperlink in die aan de afbeelding is gekoppeld.

```csharp
public string HyperlinkUrl { get; set; }
```

### Voorbeelden

Laat zien hoe u een hyperlink aan een afbeelding koppelt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://afbeelding.com"};

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### Zie ook

* class [Image](../)
* naamruimte [Aspose.Note](../../image/)
* montage [Aspose.Note](../../../)


