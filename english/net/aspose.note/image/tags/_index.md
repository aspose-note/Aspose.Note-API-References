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
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize Outline class object
Outline outline = new Outline(doc);

// Initialize OutlineElement class object
OutlineElement outlineElem = new OutlineElement(doc);

// Load an image
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

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


