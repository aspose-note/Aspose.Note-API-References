---
title: ParagraphStyle
second_title: Aspose.Note for .NET API Reference
description: 
type: docs
weight: 460
url: /net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

Text style settings to be used if there is no matching TextStyle object in [`Styles`](../richtext/styles) collection either this object doesn't specify a needed setting.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## Constructors

| Name | Description |
| --- | --- |
| [ParagraphStyle](paragraphstyle)() | Initializes a new instance of the [`ParagraphStyle`](../paragraphstyle) class. |

## Properties

| Name | Description |
| --- | --- |
| static [Default](default) { get; } | Gets the ParagraphStyle with default settings. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](equals)(object) | Determines whether the specified object is equal to the current object. |
| [Equals](equals)(ParagraphStyle) | Determines whether the specified object is equal to the current object. |

### Examples

Let's format table for better perception. Make header row bold and italic, highlight every even row using LightGray color.

```csharp
string dataDir = RunExamples.GetDataDir_Tables();

// Load the document into Aspose.Note.
Document document = new Document(dataDir + "ChangeTableStyleIn.one");

// Get a list of table nodes
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    SetRowStyle(table.First(), Color.DarkGray, true, true);

    // Highlight first row after head.
    var flag = false;
    foreach (var row in table.Skip(1))
    {
        SetRowStyle(row, flag ? Color.LightGray : Color.Empty, false, false);

        flag = !flag;
    }
}

document.Save(Path.Combine(dataDir, "ChangeTableStyleOut.one"));
```

Manipulate by text format using paragraph style.

```csharp
var document = new Document();
var page = new Page(document);
var outline = new Outline(document);
var outlineElem = new OutlineElement(document);

var text = new RichText(document)
            {
                Text = $"DefaultParagraphFontAndSize{Environment.NewLine}OnlyDefaultParagraphFont{Environment.NewLine}OnlyDefaultParagraphFontSize",
                ParagraphStyle = new ParagraphStyle()
                                    {
                                        FontName = "Courier New",
                                        FontSize = 20
                                    }
            };

// Font and font size are from text.ParagraphStyle
text.Styles.Add(new TextStyle()
                        {
                            RunIndex = 27
                        });

// Only font is from text.ParagraphStyle
text.Styles.Add(new TextStyle()
                        {
                            FontSize = 14,
                            RunIndex = 53
                        });

// Only font size is from text.ParagraphStyle
text.Styles.Add(new TextStyle()
                        {
                            FontName = "Verdana",
                            RunIndex = text.Text.Length
                        });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
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

* class [Style](../style)
* namespace [Aspose.Note](../../aspose.note)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
