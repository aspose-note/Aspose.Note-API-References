---
title: Class Image
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Image class. Represents an Image
type: docs
weight: 250
url: /net/aspose.note/image/
---
## Image class

Represents an Image.

```csharp
public sealed class Image : CompositeNode<Loop>, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Constructors

| Name | Description |
| --- | --- |
| [Image](image/#constructor)() | Initializes a new instance of the `Image` class. |
| [Image](image/#constructor_1)(string) | Initializes a new instance of the `Image` class. |
| [Image](image/#constructor_2)(string, Stream) | Initializes a new instance of the `Image` class. |
| [Image](image/#constructor_3)(string, string, string) | Initializes a new instance of the `Image` class. |

## Properties

| Name | Description |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | Gets or sets the alignment. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | Gets or sets a body an alternative text for the image. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | Gets or sets a title of alternative text for the image. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | Gets the image data store. |
| [Document](../../aspose.note/node/document/) { get; } | Gets the document of the node. |
| [FileName](../../aspose.note/image/filename/) { get; } | Gets the file name. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | Gets the path to the image file. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Format](../../aspose.note/image/format/) { get; } | Gets the image's format. |
| [Height](../../aspose.note/image/height/) { get; set; } | Gets or sets the height. This is the real height of the image in the MS OneNote document. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | Gets or sets the horizontal offset. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | Gets or sets the hyperlink associated with the image. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | Gets whether the image is a background image. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | Gets or sets last modified time. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Gets the next node at the same node tree level. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Gets the node type. |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | Gets the original height. This is the original width of the image, before resizing. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | Gets the original width. This is the original width of the image, before resizing. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Gets the parent node. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Gets the previous node at the same node tree level. |
| [Tags](../../aspose.note/image/tags/) { get; } | Gets the list of all tags of a paragraph. |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | Gets or sets the vertical offset. |
| [Width](../../aspose.note/image/width/) { get; set; } | Gets or sets the width. This is the real width of the image in the MS OneNote document. |

## Methods

| Name | Description |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | Accepts the visitor of the node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Loop&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Loop[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Replace](../../aspose.note/image/replace/)(Image) | Replaces the current image data with the data from the provided Image object. |

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

Shows how to get an image from a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Get all Image nodes
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Save image bytes to a file
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Shows how to get image's meta information.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Get all Image nodes
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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

Shows how to add an image from file to a document with user defined properties.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Load document from the stream.
Document doc = new Document(dataDir + "Aspose.one");

// Get the first page of the document.
Aspose.Note.Page page = doc.FirstChild;

// Load an image from the file.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Change the image's size according to your needs (optional).
                              Width = 100,
                              Height = 100,

                              // Set the image's location in the page (optional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Set image alignment
                              Alignment = HorizontalAlignment.Right
                          };

// Add the image to the page.
page.AppendChildLast(image);
```

Shows how to add an image from stream to a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Load the second image using the image name, extension and stream.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Set image alignment
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Shows how to add an image from file to a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Images();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize Outline class object and set offset properties
Outline outline = new Outline(doc);

// Initialize OutlineElement class object
OutlineElement outlineElem = new OutlineElement(doc);

// Load an image by the file path.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Set image alignment
                              Alignment = HorizontalAlignment.Right
                          };

// Add image
outlineElem.AppendChildLast(image);

// Add outline elements
outline.AppendChildLast(outlineElem);

// Add Outline node
page.AppendChildLast(outline);

// Add Page node
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### See Also

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Loop](../loop/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


