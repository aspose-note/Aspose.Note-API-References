---
title: Class ImageBinarizationOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.ImageBinarizationOptions कक्ष. इमेज के बनरइज़ेशन के लए वकल्प.
type: docs
weight: 710
url: /hi/net/aspose.note.saving/imagebinarizationoptions/
---
## ImageBinarizationOptions class

इमेज के बिनराइज़ेशन के लिए विकल्प.

```csharp
public class ImageBinarizationOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ImageBinarizationOptions](imagebinarizationoptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [BinarizationMethod](../../aspose.note.saving/imagebinarizationoptions/binarizationmethod/) { get; set; } | बिनराइजेशन विधि प्राप्त या सेट करता है। डिफ़ॉल्ट मान हैFixedThreshold . |
| [BinarizationThreshold](../../aspose.note.saving/imagebinarizationoptions/binarizationthreshold/) { get; set; } | फिक्स्ड थ्रेशोल्ड बाइनराइजेशन विधि के लिए थ्रेशोल्ड मान प्राप्त या सेट करता है। डिफ़ॉल्ट मान 128. है |

### उदाहरण

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

* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


