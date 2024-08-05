---
title: Class Title
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Title class. Represents a title
type: docs
weight: 1050
url: /net/aspose.note/title/
---
## Title class

Represents a title.

```csharp
public sealed class Title : CompositeNodeBase, ICompositeNode<RichText>, IPageChildNode
```

## Constructors

| Name | Description |
| --- | --- |
| [Title](title/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Gets the document of the node. |
| [HorizontalOffset](../../aspose.note/title/horizontaloffset/) { get; set; } | Gets or sets the horizontal offset. |
| override [IsComposite](../../aspose.note/title/iscomposite/) { get; } | Gets a value indicating whether this node is composite. If true the node can have child nodes. |
| [LastModifiedTime](../../aspose.note/title/lastmodifiedtime/) { get; set; } | Gets or sets the last modified time. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Gets the next node at the same node tree level. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Gets the node type. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Gets the parent node. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Gets the previous node at the same node tree level. |
| [TitleDate](../../aspose.note/title/titledate/) { get; set; } | Gets or sets a string representation of the date in the title. |
| [TitleText](../../aspose.note/title/titletext/) { get; set; } | Gets or sets the text of the title. |
| [TitleTime](../../aspose.note/title/titletime/) { get; set; } | Gets or sets a string representation of the time in the title. |
| [VerticalOffset](../../aspose.note/title/verticaloffset/) { get; set; } | Gets or sets the vertical offset. |

## Methods

| Name | Description |
| --- | --- |
| override [Accept](../../aspose.note/title/accept/)(DocumentVisitor) | Accepts the visitor of the node. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/title/getchildnodes/#getchildnodes_1)() | Get all child nodes by the node type. |
| [GetEnumerator](../../aspose.note/title/getenumerator/)() | Returns an enumerator that iterates through child nodes of the `Title`. |

## Examples

Shows how to edit page's history.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Pages();

// Load OneNote document and get first child           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

Shows how to set a title for a page.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

Shows how to create a document and save it in html format using default options.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialize OneNote document
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// Default style for all text in the document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// Save into HTML format
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

Shows how to create a document and save in html format specified range of pages.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialize OneNote document
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Default style for all text in the document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Save into HTML format
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Shows how to create a document with titled page.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Create an object of the Document class
Document doc = new Aspose.Note.Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Default style for all text in the document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Set page title properties
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Append Page node in the document
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

Shows how to save a document in different formats.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initialize the new Document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Initialize the new Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Default style for all text in the document.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Append page node
doc.AppendChildLast(page);

// Save OneNote document in different formats, set text font size and detect layout changes manually.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### See Also

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* class [RichText](../richtext/)
* interface [IPageChildNode](../ipagechildnode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


