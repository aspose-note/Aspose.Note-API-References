---
title: Style.FontColor
second_title: Aspose.Note for .NET API Reference
description: Style property. Gets or sets the font color
type: docs
weight: 10
url: /net/aspose.note/style/fontcolor/
---
## Style.FontColor property

Gets or sets the font color.

```csharp
public Color FontColor { get; set; }
```

## Examples

Shows how to change style for a text.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Get a particular RichText node
RichText richText = document.GetChildNodes<RichText>().First();

foreach (var run in richText.TextRuns)
{
    // Set font color
    run.Style.FontColor = Color.Yellow;

    // Set highlight color
    run.Style.Highlight = Color.Blue;

    // Set font size
    run.Style.FontSize = 20;
}
```

Shows how to apply Dark theme style to a Document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

Shows how to insert new list with chinese numbering.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Initialize OneNote document
Document doc = new Document();

// Initialize OneNote page
Page page = new Page();
Outline outline = new Outline();

// Apply text style settings
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Numbers in the same outline are automatically incremented.
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
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
Document doc = new Document();

// Initialize Page class object
Page page = new Page();

// Initialize Outline class object
Outline outline = new Outline();

// Initialize TextStyle class object and set formatting properties
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialize OutlineElement class objects and apply bullets
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };

// Initialize RichText class object and apply text style
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(  ) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
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
Page page = new Page();

// Initialize Outline class object
Outline outline = new Outline();

// Initialize TextStyle class object and set formatting properties
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Initialize OutlineElement class objects and apply numbering
// Numbers in the same outline are automatically incremented.
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
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

Shows how to bind a hyperlink to a text.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tasks();

// Create an object of the Document class
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Add outline elements
outline.AppendChildLast(outlineElem);

// Initialize Title class object
Title title = new Title() { TitleText = titleText };

// Initialize Page class object
Page page = new Note.Page() { Title = title };

// Add Outline node
page.AppendChildLast(outline);

// Add Page node
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

Shows how to compose a table having text with various styles.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var headerText = new RichText() { ParagraphStyle = new ParagraphStyle() { FontSize = 18, IsBold = true }, Alignment = HorizontalAlignment.Center }
                    .Append("Super contest for suppliers.");

var page = new Page();
var outline = page.AppendChildLast(new Outline() { HorizontalOffset = 50 });
outline.AppendChildLast(new OutlineElement()).AppendChildLast(headerText);

// Summary text before table
var bodyTextHeader = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
bodyTextHeader.Append("This is the final ranking of proposals got from our suppliers.");

var ranking = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new Table());
var headerRow = ranking.AppendChildFirst(new TableRow());

var headerStyle = ParagraphStyle.Default;
headerStyle.IsBold = true;

// Let's add a set of columns and a header row
var backGroundColor = Color.LightGray;
foreach (var header in new[] { "Supplier", "Contacts", "Score A", "Score B", "Score C", "Final score", "Attached materials", "Comments" })
{
    ranking.Columns.Add(new TableColumn());
    headerRow.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
             .AppendChildLast(new OutlineElement())
             .AppendChildLast(new RichText() { ParagraphStyle = headerStyle })
                .Append(header);
}

// Let's 5 empty rows. Rows have interchanging background color
for (int i = 0; i < 5; i++)
{
    backGroundColor = backGroundColor.IsEmpty ? Color.LightGray : Color.Empty;

    var row = ranking.AppendChildLast(new TableRow());
    for (int j = 0; j < ranking.Columns.Count(); j++)
    {
        row.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
           .AppendChildLast(new OutlineElement())
           .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
    }
}

// Let's add some template for content in 'Contacts' column
foreach (var row in ranking.Skip(1))
{
    var contactsCell = row.ElementAt(1);
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("Web: ").Append("link", new TextStyle() { HyperlinkAddress = "www.link.com", IsHyperlink = true });
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("E-mail: ").Append("mail", new TextStyle() { HyperlinkAddress = "mailto:hi@link.com", IsHyperlink = true });
}

var d = new Document();
d.AppendChildLast(page);
d.Save(Path.Combine(dataDir, "ComposeTable_out.one"));
```

### See Also

* class [Style](../)
* namespace [Aspose.Note](../../style/)
* assembly [Aspose.Note](../../../)


