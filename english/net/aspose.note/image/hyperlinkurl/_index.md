---
title: Image.HyperlinkUrl
second_title: Aspose.Note for .NET API Reference
description: Image property. Gets or sets the hyperlink associated with the image
type: docs
weight: 110
url: /net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

Gets or sets the hyperlink associated with the image.

```csharp
public string HyperlinkUrl { get; set; }
```

## Examples

Shows how to bind a hyperlink to an image.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### See Also

* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


