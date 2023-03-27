---
title: AttachedFile
second_title: Aspose.Note for .NET API Reference
description: Represents an attached file.
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
| [AttachedFile](attachedfile#constructor)() | Initializes a new instance of the [`AttachedFile`](../attachedfile) class. |
| [AttachedFile](attachedfile#constructor_1)(string) | Initializes a new instance of the [`AttachedFile`](../attachedfile) class. |
| [AttachedFile](attachedfile#constructor_2)(string, Stream) | Initializes a new instance of the [`AttachedFile`](../attachedfile) class. |
| [AttachedFile](attachedfile#constructor_3)(string, Stream, ImageFormat) | Initializes a new instance of the [`AttachedFile`](../attachedfile) class. |
| [AttachedFile](attachedfile#constructor_4)(string, Stream, Stream, ImageFormat) | Initializes a new instance of the [`AttachedFile`](../attachedfile) class. |

## Properties

| Name | Description |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment) { get; set; } | Gets or sets the alignment. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription) { get; set; } | Gets or sets a body an alternative text for the icon of the attached file. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle) { get; set; } | Gets or sets a title of alternative text for the icon of the attached file. |
| [Bytes](../../aspose.note/attachedfile/bytes) { get; } | Gets the binary data for an embedded file. |
| [Document](../../aspose.note/node/document) { get; } | Gets the document of the node. |
| [Extension](../../aspose.note/attachedfile/extension) { get; } | Gets the extension of an embedded file. |
| [FileName](../../aspose.note/attachedfile/filename) { get; } | Gets the name of the embedded file. |
| [FilePath](../../aspose.note/attachedfile/filepath) { get; } | Gets the path to the original file. |
| [Height](../../aspose.note/attachedfile/height) { get; } | Gets the original height of the embedded file icon. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset) { get; set; } | Gets or sets the horizontal offset. |
| [Icon](../../aspose.note/attachedfile/icon) { get; } | Gets the binary data for the icon that is associated with the embedded file. |
| [IconExtension](../../aspose.note/attachedfile/iconextension) { get; } | Gets the extension of the icon. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Gets a value indicating whether this node is composite. If true the node can have child nodes. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout) { get; set; } | Gets or sets a value indicating whether the view of the file is printout. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser) { get; set; } | Gets or sets a value indicating whether the value of the size of the icon was explicitly updated by the user. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime) { get; set; } | Gets or sets the last modified time. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight) { get; set; } | Gets or sets the maximum height to display the embedded file icon. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth) { get; set; } | Gets or sets the maximum width to display the embedded file icon. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Gets the next node at the same node tree level. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Gets the node type. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Gets the parent node. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Gets the previous node at the same node tree level. |
| [Tags](../../aspose.note/attachedfile/tags) { get; } | Gets the list of all tags of a paragraph. |
| [Text](../../aspose.note/attachedfile/text) { get; set; } | Gets or sets the text representation of the embedded file. The string MUST NOT contain any characters of the value 10 (line feed) or 13 (carriage return). |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset) { get; set; } | Gets or sets the vertical offset. |
| [Width](../../aspose.note/attachedfile/width) { get; } | Gets the original width of the embedded file icon. |

## Methods

| Name | Description |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept)(DocumentVisitor) | Accepts the visitor of the node. |

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
