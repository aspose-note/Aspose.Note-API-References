---
title: SaveOptions.PageCount
second_title: Aspose.Note .NET API संदर्भ के लिए
description: SaveOptions संपत्त. सहेजे जने वले पृष्ठं क संख्य प्रप्त करत है य सेट करत है डफ़ल्ट रूप से हैMaxValue जसक मतलब है क दस्तवेज़ के सभ पेज रेंडर कए जएंगे.
type: docs
weight: 20
url: /hi/net/aspose.note.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

सहेजे जाने वाले पृष्ठों की संख्या प्राप्त करता है या सेट करता है। डिफ़ॉल्ट रूप से हैMaxValue जिसका मतलब है कि दस्तावेज़ के सभी पेज रेंडर किए जाएंगे.

```csharp
public int PageCount { get; set; }
```

### उदाहरण

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

### यह सभी देखें

* class [SaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../saveoptions/)
* सभा [Aspose.Note](../../../)


