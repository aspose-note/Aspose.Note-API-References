---
title: Image.Tags
second_title: Aspose.Note for .NET API Reference
description: Image property. Gets the list of all tags of a paragraph
type: docs
weight: 160
url: /net/aspose.note/image/tags/
---
## Image.Tags property

Gets the list of all tags of a paragraph.

```csharp
public List<ITag> Tags { get; }
```

## Examples

Shows how to add new image with tag.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Page page = new Page();

// Initialize Outline class object
Outline outline = new Outline();

// Initialize OutlineElement class object
OutlineElement outlineElem = new OutlineElement();

// Load an image
Image image = new Image(dataDir + "icon.jpg");

// Insert image in the document node
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Add outline element node
outline.AppendChildLast(outlineElem);

// Add outline node
page.AppendChildLast(outline);

// Add page node
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### See Also

* interface [ITag](../../itag/)
* class [Image](../)
* namespace [Aspose.Note](../../image/)
* assembly [Aspose.Note](../../../)


