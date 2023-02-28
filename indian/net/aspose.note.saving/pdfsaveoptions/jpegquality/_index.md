---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note .NET API संदर्भ के लिए
description: PdfSaveOptions संपत्त. पडएफ दस्तवेज़ के अंदर जेपईज छवयं क गुणवत्त नर्धरत करने वल मन प्रप्त य सेट करत है मन 0 से 100 तक भन्न ह सकत है जहं 0 क मतलब सबसे खरब गुणवत्त लेकन अधकतम संपड़न और 100 क मतलब सर्वत्तम गुणवत्त लेकन न्यूनतम संपड़न है
type: docs
weight: 30
url: /hi/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

पीडीएफ दस्तावेज़ के अंदर जेपीईजी छवियों की गुणवत्ता निर्धारित करने वाला मान प्राप्त या सेट करता है। मान 0 से 100 तक भिन्न हो सकता है जहां 0 का मतलब सबसे खराब गुणवत्ता लेकिन अधिकतम संपीड़न और 100 का मतलब सर्वोत्तम गुणवत्ता लेकिन न्यूनतम संपीड़न है।

```csharp
public int JpegQuality { get; set; }
```

### टिप्पणियों

डिफ़ॉल्ट मान 90. है

### उदाहरण

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

### यह सभी देखें

* class [PdfSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../pdfsaveoptions/)
* सभा [Aspose.Note](../../../)


