---
title: Image.AlternativeTextTitle
second_title: Aspose.Note für .NET-API-Referenz
description: Image eigendom. Ruft einen alternativen Texttitel für das Bild ab oder legt ihn fest.
type: docs
weight: 40
url: /de/net/aspose.note/image/alternativetexttitle/
---
## Image.AlternativeTextTitle property

Ruft einen alternativen Texttitel für das Bild ab oder legt ihn fest.

```csharp
public string AlternativeTextTitle { get; set; }
```

### Beispiele

Zeigt, wie eine Textbeschreibung für ein Bild festgelegt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

### Siehe auch

* class [Image](../)
* namensraum [Aspose.Note](../../image/)
* Montage [Aspose.Note](../../../)


