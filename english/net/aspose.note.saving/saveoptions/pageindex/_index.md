---
title: PageIndex
second_title: Aspose.Note for .NET API Reference
description: Gets or sets the index of the first page to save. By default is 0.
type: docs
weight: 30
url: /net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

Gets or sets the index of the first page to save. By default is 0.

```csharp
public int PageIndex { get; set; }
```

### Examples

Shows how to save a document in png format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize ImageSaveOptions object 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Set page index
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Save the document as PNG.
oneFile.Save(dataDir, opts);
```

Shows how to save a document in pdf format.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Set page index of first page to be saved
                              PageIndex = 0,

                              // Set page count
                              PageCount = 1,
                          };

// Save the document as PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Shows how to save a document in pdf format using specific settings.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initialize PdfSaveOptions object
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Use Jpeg compression
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Quality for JPEG compression
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

Shows how to create a document with formatted rich text.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Page page = new Page();

// Initialize Title class object
Title title = new Title();

// Initialize TextStyle class object and set formatting properties
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

// Set page title
page.Title = title;

// Add RichText node
outlineElem.AppendChildLast(text);

// Add OutlineElement node
outline.AppendChildLast(outlineElem);

// Add Outline node
page.AppendChildLast(outline);

// Add Page node
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### See Also

* class [SaveOptions](../../saveoptions)
* namespace [Aspose.Note.Saving](../../saveoptions)
* assembly [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
