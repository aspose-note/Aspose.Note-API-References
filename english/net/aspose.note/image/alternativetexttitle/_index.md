---
title: Image.AlternativeTextTitle
second_title: Aspose.Note for .NET API Reference
description: Image property. Gets or sets a title of alternative text for the image
type: docs
weight: 40
url: /net/aspose.note/image/alternativetexttitle/
---
## Image.AlternativeTextTitle property

Gets or sets a title of alternative text for the image.

```csharp
public string AlternativeTextTitle { get; set; }
```

## Examples

Shows how to set text description for an image.

```csharp
// The path to the documents directory.
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

### See Also

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


