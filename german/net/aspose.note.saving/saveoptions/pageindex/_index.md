---
title: PageIndex
second_title: Aspose.Note für .NET-API-Referenz
description: Ruft den Index der ersten zu speichernden Seite ab oder legt ihn fest. Standardmäßig ist 0.
type: docs
weight: 30
url: /de/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

Ruft den Index der ersten zu speichernden Seite ab oder legt ihn fest. Standardmäßig ist 0.

```csharp
public int PageIndex { get; set; }
```

### Beispiele

Zeigt, wie ein Dokument im PNG-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// ImageSaveOptions-Objekt initialisieren 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Seitenindex setzen
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Speichern Sie das Dokument als PNG.
oneFile.Save(dataDir, opts);
```

Zeigt, wie ein Dokument im PDF-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions-Objekt initialisieren
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Seitenindex der ersten zu speichernden Seite setzen
                              PageIndex = 0,

                              // Seitenanzahl festlegen
                              PageCount = 1,
                          };

// Dokument als PDF speichern
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Zeigt, wie Sie ein Dokument im PDF-Format mit bestimmten Einstellungen speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions-Objekt initialisieren
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // JPEG-Komprimierung verwenden
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Qualität für JPEG-Komprimierung
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

Zeigt, wie man ein Dokument erstellt und einen bestimmten Seitenbereich im HTML-Format speichert.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote-Dokument initialisieren
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Standardstil für den gesamten Text im Dokument.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Im HTML-Format speichern
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Zeigt, wie ein Dokument mit formatiertem Rich-Text erstellt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Page page = new Page();

// Titelklassenobjekt initialisieren
Title title = new Title();

// TextStyle-Klassenobjekt initialisieren und Formatierungseigenschaften festlegen
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

// Seitentitel festlegen
page.Title = title;

// RichText-Knoten hinzufügen
outlineElem.AppendChildLast(text);

// OutlineElement-Knoten hinzufügen
outline.AppendChildLast(outlineElem);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### Siehe auch

* class [SaveOptions](../../saveoptions)
* namensraum [Aspose.Note.Saving](../../saveoptions)
* Montage [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
