---
title: TextStyle
second_title: Aspose.Note for .NET API Reference
description: 
type: docs
weight: 910
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
| static [DefaultMsOneNoteTitleDateStyle](defaultmsonenotetitledatestyle) { get; } | Gets default style for title date in MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](defaultmsonenotetitletextstyle) { get; } | Gets default style for title text in MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](defaultmsonenotetitletimestyle) { get; } | Gets default style for title time in MS OneNote. |
| [HyperlinkAddress](hyperlinkaddress) { get; set; } | Gets or sets the hyperlink address. Must be set if the value of the [`IsHyperlink`](./ishyperlink) property is true. |
| [IsHidden](ishidden) { get; set; } | Gets or sets a value indicating whether the text style is hidden. |
| [IsHyperlink](ishyperlink) { get; set; } | Gets or sets a value indicating whether the text style is hyperlink. |
| [IsMathFormatting](ismathformatting) { get; set; } | Gets or sets a value indicating whether the text style is math-formatting. |
| [Language](language) { get; set; } | Gets or sets the language of the text. |
| [RunIndex](runindex) { get; set; } | Gets or sets the run index. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](equals)(object) | Determines whether the specified object is equal to the current object. |
| [Equals](equals)(TextStyle) | Determines whether the specified object is equal to the current object. |

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

Set proofing language for a text.

```csharp
var document = new Document();
var page = new Page(document);
var outline = new Outline(document);
var outlineElem = new OutlineElement(document);

var text = new RichText(document) { Text = "United States Germany China", ParagraphStyle = ParagraphStyle.Default };
text.Styles.Add(new TextStyle()
                    {
                        Language = CultureInfo.GetCultureInfo("en-US"),
                        RunIndex = 13
                    });
text.Styles.Add(new TextStyle()
                    {
                        Language = CultureInfo.GetCultureInfo("de-DE"),
                        RunIndex = 21
                    });
text.Styles.Add(new TextStyle()
                    {
                        Language = CultureInfo.GetCultureInfo("zh-CN"),
                        RunIndex = text.Text.Length
                    });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
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

Shows how to bind a hyperlink to a text.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tasks();

// Create an object of the Document class
Document doc = new Document();

RichText titleText = new RichText(doc)
                     {
                         Text = "Title!",
                         ParagraphStyle = ParagraphStyle.Default
                     };

Outline outline = new Outline(doc)
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

                             // This style will be applied to 0-7 characters.
                             RunIndex = 8 
                         };

TextStyle textStyleHyperlink = new TextStyle
                              {
                                  // This style will be applied to 8-16 characters.
                                  RunIndex = 17,
                                  IsHyperlink = true,
                                  HyperlinkAddress = "www.google.com"
                              };

RichText text = new RichText(doc)
                {
                    Text = "This is hyperlink. This text is not a hyperlink.",
                    ParagraphStyle = ParagraphStyle.Default,
                    Styles = { textStyleRed, textStyleHyperlink }
                };

OutlineElement outlineElem = new OutlineElement(doc);
outlineElem.AppendChildLast(text);

// Add outline elements
outline.AppendChildLast(outlineElem);

// Initialize Title class object
Title title = new Title(doc) { TitleText = titleText };

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc) { Title = title };

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
