---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note .NET API संदर्भ के लिए
description: PdfSaveOptions संपत्त. पडएफ फइल में छवयं पर लगू संपड़न के प्रकर क प्रप्त य सेट करत है
type: docs
weight: 20
url: /hi/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

पीडीएफ फाइल में छवियों पर लागू संपीड़न के प्रकार को प्राप्त या सेट करता है।

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

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

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../pdfsaveoptions/)
* सभा [Aspose.Note](../../../)


