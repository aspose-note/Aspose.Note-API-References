---
title: SaveOptions.PageIndex
second_title: Aspose.Note .NET API संदर्भ के लिए
description: SaveOptions संपत्त. सहेजे जने वले पहले पृष्ठ क अनुक्रमणक प्रप्त करत है य सेट करत है डफ़ल्ट रूप से 0. है
type: docs
weight: 30
url: /hi/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

सहेजे जाने वाले पहले पृष्ठ की अनुक्रमणिका प्राप्त करता है या सेट करता है। डिफ़ॉल्ट रूप से 0. है

```csharp
public int PageIndex { get; set; }
```

### उदाहरण

दिखाता है कि दस्तावेज़ को पीएनजी प्रारूप में कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// ImageSaveOptions ऑब्जेक्ट को इनिशियलाइज़ करें 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // पेज इंडेक्स सेट करें
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// दस्तावेज़ को पीएनजी के रूप में सहेजें।
oneFile.Save(dataDir, opts);
```

दिखाता है कि पीडीएफ प्रारूप में दस्तावेज़ को कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions ऑब्जेक्ट को इनिशियलाइज़ करें
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // सहेजे जाने वाले पहले पेज का पेज इंडेक्स सेट करें
                              PageIndex = 0,

                              // पेज काउंट सेट करें
                              PageCount = 1,
                          };

// दस्तावेज़ को पीडीएफ के रूप में सहेजें
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

दिखाता है कि विशिष्ट सेटिंग्स का उपयोग करके दस्तावेज़ को पीडीएफ प्रारूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions ऑब्जेक्ट को इनिशियलाइज़ करें
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // जेपीईजी संपीड़न का प्रयोग करें
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // जेपीईजी संपीड़न के लिए गुणवत्ता
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

दिखाता है कि दस्तावेज़ कैसे बनाया जाए और HTML प्रारूप में निर्दिष्ट पृष्ठों की श्रेणी में सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote दस्तावेज़ को प्रारंभ करें
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// दस्तावेज़ में सभी पाठ के लिए डिफ़ॉल्ट शैली।
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML फॉर्मेट में सेव करें
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

स्वरूपित रिच टेक्स्ट के साथ दस्तावेज़ बनाने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Page page = new Page();

// टाइटल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Title title = new Title();

// टेक्स्ट स्टाइल क्लास ऑब्जेक्ट प्रारंभ करें और स्वरूपण गुण सेट करें
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

// पेज का शीर्षक सेट करें
page.Title = title;

// रिचटेक्स्ट नोड जोड़ें
outlineElem.AppendChildLast(text);

// आउटलाइन एलिमेंट नोड जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### यह सभी देखें

* class [SaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../saveoptions/)
* सभा [Aspose.Note](../../../)


