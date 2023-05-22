---
title: OutlineElement
second_title: Aspose.Note for .NET API Reference
description: Represents a OutlineElement.
type: docs
weight: 500
url: /net/aspose.note/outlineelement/
---
## OutlineElement class

Represents a OutlineElement.

```csharp
public sealed class OutlineElement : IndentatedNode<IOutlineElementChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## Constructors

| Name | Description |
| --- | --- |
| [OutlineElement](outlineelement)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [CreationTime](../../aspose.note/outlineelement/creationtime) { get; set; } | Gets or sets the creation time. |
| [Document](../../aspose.note/node/document) { get; } | Gets the document of the node. |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode`1/indentposition) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/outlineelement/lastmodifiedtime) { get; set; } | Gets or sets the last modified time. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Gets the next node at the same node tree level. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Gets the node type. |
| [NumberList](../../aspose.note/outlineelement/numberlist) { get; set; } | Gets or sets the style for the numbered list header. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Gets the parent node. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Gets the previous node at the same node tree level. |

## Methods

| Name | Description |
| --- | --- |
| override [Accept](../../aspose.note/outlineelement/accept)(DocumentVisitor) | Accepts the visitor of the node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;IOutlineElementChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params IOutlineElementChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### Examples

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

Shows how to retrieve information about list's formatting.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Retrieve a collection nodes of the outline element
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Iterate through each node
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Retrieve font name
        Console.WriteLine("Font Name: " + list.Font);

        // Retrieve font length
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Retrieve font size
        Console.WriteLine("Font Size: " + list.FontSize);

        // Retrieve font color
        Console.WriteLine("Font Color: " + list.FontColor);

        // Retrieve format
        Console.WriteLine("Font format: " + list.Format);

        // Check bold
        Console.WriteLine("Is bold: " + list.IsBold);

        // Check italic
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

Shows how to insert new list with chinese numbering.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Initialize OneNote document
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initialize OneNote page
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Apply text style settings
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Numbers in the same outline are automatically incremented.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Shows how to insert new bulleted lis.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Create an object of the Document class
Aspose.Note.Document doc = new Aspose.Note.Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize Outline class object
Outline outline = new Outline(doc);

// Initialize TextStyle class object and set formatting properties
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialize OutlineElement class objects and apply bullets
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Initialize RichText class object and apply text style
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Add outline elements
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Add Outline node
page.AppendChildLast(outline);
// Add Page node
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Shows how to insert new list with numbering.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize Outline class object
Outline outline = new Outline(doc);

// Initialize TextStyle class object and set formatting properties
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialize OutlineElement class objects and apply numbering
// Numbers in the same outline are automatically incremented.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Add outline elements
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Add Outline node
page.AppendChildLast(outline);

// Add Page node
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### See Also

* class [IndentatedNode&lt;T&gt;](../indentatednode-1)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IOutlineChildNode](../ioutlinechildnode)
* namespace [Aspose.Note](../../aspose.note)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
