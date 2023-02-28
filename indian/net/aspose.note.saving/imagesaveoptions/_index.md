---
title: Class ImageSaveOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.ImageSaveOptions कक्ष. दस्तवेज़ पृष्ठं क छवयं के लए प्रस्तुत करते समय अतरक्त वकल्प नर्दष्ट करने क अनुमत देत है
type: docs
weight: 720
url: /hi/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

दस्तावेज़ पृष्ठों को छवियों के लिए प्रस्तुत करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class ImageSaveOptions : SaveOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | का एक नया उदाहरण प्रारंभ करता है`ImageSaveOptions` वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | छवि के द्वैतकरण के लिए विकल्प प्राप्त या सेट करता है। |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | हो जाता है या सेट हो जाता है[`ColorMode`](./colormode/) आउटपुट छवि के लिए. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | को सहेजते समय उपयोग किए जाने वाले फ़ॉन्ट की सेटिंग प्राप्त या सेट करता है |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | सहेजे जाने वाले पृष्ठों की संख्या प्राप्त करता है या सेट करता है। डिफ़ॉल्ट रूप से हैMaxValue जिसका मतलब है कि दस्तावेज़ के सभी पेज रेंडर किए जाएंगे. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | सहेजे जाने वाले पहले पृष्ठ की अनुक्रमणिका प्राप्त करता है या सेट करता है। डिफ़ॉल्ट रूप से 0. है |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | सहेजी गई छवि की गुणवत्ता निर्धारित करने वाला मान प्राप्त या सेट करता है। |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | उत्पन्न छवियों के लिए डॉट्स प्रति इंच में रिज़ॉल्यूशन प्राप्त या सेट करता है। |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | उस प्रारूप को प्राप्त करता है जिसमें दस्तावेज़ सहेजा गया है। |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | टीआईएफएफ प्रारूप में जेनरेट की गई छवियों को सहेजते समय उपयोग करने के लिए संपीड़न के प्रकार को प्राप्त या सेट करता है। |

### उदाहरण

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

जेपीईजी प्रारूप में दस्तावेज़ को छवि के रूप में सहेजते समय छवि गुणवत्ता कैसे सेट करें दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// दस्तावेज़ को सहेजें।
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
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

दस्तावेज़ को छवि के रूप में सहेजते समय छवि रिज़ॉल्यूशन सेट करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// दस्तावेज़ को सहेजें।
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
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

निर्दिष्ट विकल्पों के साथ नोटबुक को छवि के रूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// नोटबुक को सेव करें
notebook.Save(dataDir, notebookSaveOptions);
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

छवि के रूप में चपटी नोटबुक को सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// नोटबुक को सेव करें
notebook.Save(dataDir, notebookSaveOptions);
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

* class [SaveOptions](../saveoptions/)
* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


