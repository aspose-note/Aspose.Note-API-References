---
title: AttachedFile
second_title: Aspose.Note for .NET API Reference
description: 
type: docs
weight: 10
url: /net/aspose.note/attachedfile/
---
## AttachedFile class

Represents an attached file.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Constructors

| Name | Description |
| --- | --- |
| [AttachedFile](attachedfile)() | Initializes a new instance of the [`AttachedFile`](../attachedfile) class. |
| [AttachedFile](attachedfile)(string, Stream) | Initializes a new instance of the [`AttachedFile`](../attachedfile) class. |
| [AttachedFile](attachedfile)(string, Stream, ImageFormat) | Initializes a new instance of the [`AttachedFile`](../attachedfile) class. |
| [AttachedFile](attachedfile)(string, Stream, Stream, ImageFormat) | Initializes a new instance of the [`AttachedFile`](../attachedfile) class. |

## Properties

| Name | Description |
| --- | --- |
| [Alignment](alignment) { get; set; } | Gets or sets the alignment. |
| [AlternativeTextDescription](alternativetextdescription) { get; set; } | Gets or sets a body an alternative text for the icon of the attached file. |
| [AlternativeTextTitle](alternativetexttitle) { get; set; } | Gets or sets a title of alternative text for the icon of the attached file. |
| [Bytes](bytes) { get; } | Gets the binary data for an embedded file. |
| [Extension](extension) { get; } | Gets the extension of an embedded file. |
| [FileName](filename) { get; } | Gets the name of the embedded file. |
| [FilePath](filepath) { get; } | Gets the path to the original file. |
| [Height](height) { get; } | Gets the original height of the embedded file icon. |
| [HorizontalOffset](horizontaloffset) { get; set; } | Gets or sets the horizontal offset. |
| [Icon](icon) { get; } | Gets the binary data for the icon that is associated with the embedded file. |
| [IconExtension](iconextension) { get; } | Gets the extension of the icon. |
| [IsPrintout](isprintout) { get; set; } | Gets or sets a value indicating whether the view of the file is printout. |
| [IsSizeSetByUser](issizesetbyuser) { get; set; } | Gets or sets a value indicating whether the value of the size of the icon was explicitly updated by the user. |
| [LastModifiedTime](lastmodifiedtime) { get; set; } | Gets or sets the last modified time. |
| [MaxHeight](maxheight) { get; set; } | Gets or sets the maximum height to display the embedded file icon. |
| [MaxWidth](maxwidth) { get; set; } | Gets or sets the maximum width to display the embedded file icon. |
| [Tags](tags) { get; } | Gets the list of all tags of a paragraph. |
| [Text](text) { get; set; } | Gets or sets the text representation of the embedded file. The string MUST NOT contain any characters of the value 10 (line feed) or 13 (carriage return). |
| [VerticalOffset](verticaloffset) { get; set; } | Gets or sets the vertical offset. |
| [Width](width) { get; } | Gets the original width of the embedded file icon. |

## Methods

| Name | Description |
| --- | --- |
| override [Accept](accept)(DocumentVisitor) | Accepts the visitor of the node. |

### Examples

Shows how to get content of an attached file.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Attachments();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Get a list of attached file nodes
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Iterate through all nodes
foreach (AttachedFile file in nodes)
{
    // Load attached file to a stream object
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Create a local file
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Copy file stream
            CopyStream(outputStream, fileStream);
        }
    }
}
```

Shows how to add a file to a document by using filepath.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Attachments();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize Outline class object
Outline outline = new Outline(doc);

// Initialize OutlineElement class object
OutlineElement outlineElem = new OutlineElement(doc);

// Initialize AttachedFile class object
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Add attached file
outlineElem.AppendChildLast(attachedFile);

// Add outline element node
outline.AppendChildLast(outlineElem);

// Add outline node
page.AppendChildLast(outline);

// Add page node
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Shows how to add a file from a stream to a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Attachments();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize Outline class object
Outline outline = new Outline(doc);

// Initialize OutlineElement class object
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Initialize AttachedFile class object and also pass its icon path
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Add attached file
    outlineElem.AppendChildLast(attachedFile);
}

// Add outline element node
outline.AppendChildLast(outlineElem);

// Add outline node
page.AppendChildLast(outline);

// Add page node
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### See Also

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* namespace [Aspose.Note](../../aspose.note)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
