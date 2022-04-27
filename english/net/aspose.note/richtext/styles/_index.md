---
title: Styles
second_title: Aspose.Note for .NET API Reference
description: 
type: docs
weight: 80
url: /net/aspose.note/richtext/styles/
---
## RichText.Styles property

Gets the styles.

```csharp
public IList<TextStyle> Styles { get; }
```

### Examples

Shows how to change style for a text.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Load the document into Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Get a particular RichText node
RichText richText = document.GetChildNodes<RichText>().First();

foreach (TextStyle style in richText.Styles)
{
    // Set font color
    style.FontColor = Color.Yellow;

    // Set highlight color
    style.Highlight = Color.Blue;

    // Set font size
    style.FontSize = 20;
}
```

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

* class [TextStyle](../../textstyle)
* class [RichText](../../richtext)
* namespace [Aspose.Note](../../richtext)
* assembly [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
