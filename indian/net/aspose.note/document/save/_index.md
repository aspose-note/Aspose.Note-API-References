---
title: Document.Save
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document तरक. OneNote दस्तवेज़ क फ़इल में सहेजत है.
type: docs
weight: 140
url: /hi/net/aspose.note/document/save/
---
## Save(string) {#save_3}

OneNote दस्तावेज़ को फ़ाइल में सहेजता है.

```csharp
public void Save(string fileName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | String | फ़ाइल का पूरा नाम। यदि निर्दिष्ट पूर्ण नाम वाली फ़ाइल पहले से मौजूद है, तो मौजूदा फ़ाइल अधिलेखित हो जाती है. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### उदाहरण

दस्तावेज़ को सहेजने का तरीका दिखाता है।

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Save(Stream) {#save}

OneNote दस्तावेज़ को स्ट्रीम में सहेजता है.

```csharp
public void Save(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | System.IO.Stream जहां दस्तावेज़ सहेजा जाएगा. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

OneNote दस्तावेज़ को निर्दिष्ट स्वरूप में फ़ाइल में सहेजता है.

```csharp
public void Save(string fileName, SaveFormat format)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | String | फ़ाइल का पूरा नाम। यदि निर्दिष्ट पूर्ण नाम वाली फ़ाइल पहले से मौजूद है, तो मौजूदा फ़ाइल अधिलेखित हो जाती है. |
| format | SaveFormat | वह प्रारूप जिसमें दस्तावेज़ को सहेजना है। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### उदाहरण

दिखाता है कि SaveFormat गणन का उपयोग करके दस्तावेज़ को कैसे सहेजना है।

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

किसी दस्तावेज़ को GIF प्रारूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// दस्तावेज़ को GIF के रूप में सहेजें।
oneFile.Save(dataDir, SaveFormat.Gif);
```

### यह सभी देखें

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

निर्दिष्ट प्रारूप में एक स्ट्रीम में OneNote दस्तावेज़ सहेजता है।

```csharp
public void Save(Stream stream, SaveFormat format)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | System.IO.Stream जहां दस्तावेज़ सहेजा जाएगा. |
| format | SaveFormat | वह प्रारूप जिसमें दस्तावेज़ को सहेजना है। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### उदाहरण

दिखाता है कि डिफ़ॉल्ट सेटिंग्स का उपयोग करके किसी दस्तावेज़ को पीडीएफ प्रारूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// दस्तावेज़ को पीडीएफ के रूप में सहेजें
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

किसी दस्तावेज़ को स्ट्रीम में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// स्ट्रीम की स्थिति को वापस शून्य पर रिवाइंड करें ताकि यह अगले पाठक के लिए तैयार हो।
dstStream.Seek(0, SeekOrigin.Begin);
```

किसी दस्तावेज़ में डार्क थीम शैली को लागू करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### यह सभी देखें

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

निर्दिष्ट सहेजें विकल्पों का उपयोग करके OneNote दस्तावेज़ को फ़ाइल में सहेजता है.

```csharp
public void Save(string fileName, SaveOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | String | फ़ाइल का पूरा नाम। यदि निर्दिष्ट पूर्ण नाम वाली फ़ाइल पहले से मौजूद है, तो मौजूदा फ़ाइल अधिलेखित हो जाती है. |
| options | SaveOptions | दस्तावेज़ को फ़ाइल में सहेजे जाने के विकल्पों को निर्दिष्ट करता है. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### उदाहरण

दिखाता है कि OneSaveOptions का उपयोग करके किसी दस्तावेज़ को कैसे सहेजना है।

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

दिखाता है कि कैसे SaveFormat का उपयोग करके दस्तावेज़ को जेपीईजी प्रारूप में छवि के रूप में सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// दस्तावेज़ को सहेजें।
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

ImageSaveOptions का उपयोग करके किसी दस्तावेज़ को छवि के रूप में Bmp प्रारूप में सहेजना दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// दस्तावेज़ को सहेजें।
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

लेटर पेज लेआउट के साथ पीडीएफ प्रारूप में दस्तावेज़ को कैसे सहेजना है, दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// दस्तावेज़ को सहेजें।
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

दिखाता है कि ऊंचाई सीमा के बिना A4 पेज लेआउट के साथ पीडीएफ प्रारूप में दस्तावेज़ को कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// दस्तावेज़ को सहेजें।
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

दस्तावेज़ को ग्रेस्केल छवि के रूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// दस्तावेज़ को GIF के रूप में सहेजें।
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

दिखाता है कि पैकबिट्स संपीड़न का उपयोग करके किसी दस्तावेज़ को टिफ़ प्रारूप में छवि के रूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// दस्तावेज़ को सहेजें।
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

दिखाता है कि जेपीईजी संपीड़न का उपयोग करके दस्तावेज़ को टिफ़ प्रारूप में छवि के रूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// दस्तावेज़ को सहेजें।
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

दिखाता है कि CCITT Group 3 फ़ैक्स संपीड़न का उपयोग करके किसी दस्तावेज़ को टिफ़ प्रारूप में छवि के रूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// दस्तावेज़ को सहेजें।
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
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

दिखाता है कि ओत्सु की विधि का उपयोग करके किसी दस्तावेज़ को बाइनरी इमेज के रूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// दस्तावेज़ को GIF के रूप में सहेजें।
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

दिखाता है कि फिक्स्ड थ्रेशोल्ड का उपयोग करके किसी दस्तावेज़ को बाइनरी इमेज के रूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// दस्तावेज़ को GIF के रूप में सहेजें।
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### यह सभी देखें

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

निर्दिष्ट सहेजें विकल्पों का उपयोग करके OneNote दस्तावेज़ को स्ट्रीम में सहेजता है.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | System.IO.Stream जहां दस्तावेज़ सहेजा जाएगा. |
| options | SaveOptions | दस्तावेज़ को स्ट्रीम में सहेजे जाने के विकल्पों को निर्दिष्ट करता है. |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | दस्तावेज़ संरचना विनिर्देश का उल्लंघन करती है। |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | अनुरोधित सहेजें प्रारूप समर्थित नहीं है। |

### उदाहरण

निर्दिष्ट डिफ़ॉल्ट फ़ॉन्ट का उपयोग करके दस्तावेज़ को पीडीएफ प्रारूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// दस्तावेज़ को पीडीएफ के रूप में सहेजें
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

फ़ाइल से डिफ़ॉल्ट फ़ॉन्ट का उपयोग करके पीडीएफ प्रारूप में दस्तावेज़ को कैसे सहेजना है, दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// दस्तावेज़ को पीडीएफ के रूप में सहेजें
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

दिखाता है कि स्ट्रीम से डिफ़ॉल्ट फ़ॉन्ट का उपयोग करके किसी दस्तावेज़ को पीडीएफ प्रारूप में कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// दस्तावेज़ को पीडीएफ के रूप में सहेजें
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### यह सभी देखें

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


