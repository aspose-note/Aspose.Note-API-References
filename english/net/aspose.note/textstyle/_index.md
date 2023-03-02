---
title: TextStyle
second_title: Aspose.Note for .NET API Reference
description: Specifies the text style.
type: docs
weight: 1010
url: /net/aspose.note/textstyle/
---
## TextStyle class

Specifies the text style.

```csharp
public sealed class TextStyle : Style
```

## Constructors

| Name | Description |
| --- | --- |
| [TextStyle](textstyle)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default) { get; } | Gets the style with "en-US" culture. |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle) { get; } | Gets default style for title date in MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle) { get; } | Gets default style for title text in MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle) { get; } | Gets default style for title time in MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor) { get; set; } | Gets or sets the font color. |
| [FontName](../../aspose.note/style/fontname) { get; set; } | Gets or sets the font name. |
| [FontSize](../../aspose.note/style/fontsize) { get; set; } | Gets or sets the font size. |
| [FontStyle](../../aspose.note/style/fontstyle) { get; } | Gets the font style. |
| [Highlight](../../aspose.note/style/highlight) { get; set; } | Gets or sets the highlight color. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress) { get; set; } | Gets or sets the hyperlink address. Must be set if the value of the [`IsHyperlink`](./ishyperlink) property is true. |
| [IsBold](../../aspose.note/style/isbold) { get; set; } | Gets or sets a value indicating whether the text style is bold. |
| [IsHidden](../../aspose.note/textstyle/ishidden) { get; set; } | Gets or sets a value indicating whether the text style is hidden. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink) { get; set; } | Gets or sets a value indicating whether the text style is hyperlink. |
| [IsItalic](../../aspose.note/style/isitalic) { get; set; } | Gets or sets a value indicating whether the text style is italic. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting) { get; set; } | Gets or sets a value indicating whether the text style is math-formatting. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough) { get; set; } | Gets or sets a value indicating whether the text style is strikethrough. |
| [IsSubscript](../../aspose.note/style/issubscript) { get; set; } | Gets or sets a value indicating whether the text style is subscript. |
| [IsSuperscript](../../aspose.note/style/issuperscript) { get; set; } | Gets or sets a value indicating whether the text style is superscript. |
| [IsUnderline](../../aspose.note/style/isunderline) { get; set; } | Gets or sets a value indicating whether the text style is underline. |
| [Language](../../aspose.note/textstyle/language) { get; set; } | Gets or sets the language of the text. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals#equals_1)(object) | Determines whether the specified object is equal to the current object. |
| [Equals](../../aspose.note/textstyle/equals#equals)(TextStyle) | Determines whether the specified object is equal to the current object. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode)() | Serves as a hash function for the type. |

### Examples

Let's emphasize page's titles among other headers by increasing font's size.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Iterate through page's titles.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

Let's emphasize latest text's changes by highlighting.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Get RichText nodes modified last week.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Set highlight color
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Set highlight color
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

Set proofing language for a text.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

Manipulate by text format using paragraph style.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
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

### See Also

* class [Style](../style)
* namespace [Aspose.Note](../../aspose.note)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
