---
title: SaveOptions.PageIndex
second_title: Aspose.Note för .NET API-referens
description: SaveOptions fast egendom. Hämtar eller ställer in indexet för den första sidan som ska sparas. Som standard är 0.
type: docs
weight: 30
url: /sv/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

Hämtar eller ställer in indexet för den första sidan som ska sparas. Som standard är 0.

```csharp
public int PageIndex { get; set; }
```

### Exempel

Visar hur man sparar ett dokument i png-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initiera ImageSaveOptions-objekt 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Ställ in sidindex
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Spara dokumentet som PNG.
oneFile.Save(dataDir, opts);
```

Visar hur man sparar ett dokument i pdf-format.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Initiera PdfSaveOptions-objekt
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Ställ in sidindex för första sidan som ska sparas
                              PageIndex = 0,

                              // Ställ in antal sidor
                              PageCount = 1,
                          };

// Spara dokumentet som PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Visar hur man sparar ett dokument i pdf-format med specifika inställningar.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Initiera PdfSaveOptions-objekt
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Använd Jpeg-komprimering
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Kvalitet för JPEG-komprimering
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Visar hur man skapar ett dokument och sparar i html-format specificerat antal sidor.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Initiera OneNote-dokument
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standardstil för all text i dokumentet.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Spara i HTML-format
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Visar hur man skapar ett dokument med formaterad rik text.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera Sidklassobjekt
Page page = new Page();

// Initiera Title-klassobjekt
Title title = new Title();

// Initiera TextStyle-klassobjektet och ställ in formateringsegenskaper
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

// Ställ in sidtitel
page.Title = title;

// Lägg till RichText-nod
outlineElem.AppendChildLast(text);

// Lägg till OutlineElement-nod
outline.AppendChildLast(outlineElem);

// Lägg till Outline-nod
page.AppendChildLast(outline);

// Lägg till sidnod
doc.AppendChildLast(page);

// Spara OneNote-dokument
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### Se även

* class [SaveOptions](../)
* namnutrymme [Aspose.Note.Saving](../../saveoptions/)
* hopsättning [Aspose.Note](../../../)


