---
title: Class NumberList
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.NumberList class. Represents the numbered or bulleted list
type: docs
weight: 510
url: /net/aspose.note/numberlist/
---
## NumberList class

Represents the numbered or bulleted list.

```csharp
public class NumberList
```

## Constructors

| Name | Description |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | Initializes a new instance of the `NumberList` class. This instance represents a bulleted list. |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | Initializes a new instance of the `NumberList` class. This instance represents a numbered list. |

## Properties

| Name | Description |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | Gets or sets the name of the font. |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | Gets or sets the font color. |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | Gets or sets the font size. |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | Gets or sets the format of the line header. For bulleted lists represents a bullet symbol. |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | Gets or sets a value indicating whether the text style is bold. |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | Gets or sets a value indicating whether the text style is italic. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | Gets or sets the last modified time. |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | Gets or sets the number format used for a group of automatically numbered objects. Should be null for bulleted lists. |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | Gets or sets the numeric value that overrides the automatic number value of the list item. |

## Methods

| Name | Description |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | Determines whether the specified object is equal to the current object. |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | Determines whether the specified object is equal to the current object. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | Serves as a hash function for the type. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | Gets the numbered list header. |

## Examples

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

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


