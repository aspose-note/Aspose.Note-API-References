---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note .NET API संदर्भ के लिए
description: ImageBinarizationOptions संपत्त. फक्स्ड थ्रेशल्ड बइनरइजेशन वध के लए थ्रेशल्ड मन प्रप्त य सेट करत है डफ़ल्ट मन 128. है
type: docs
weight: 30
url: /hi/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

फिक्स्ड थ्रेशोल्ड बाइनराइजेशन विधि के लिए थ्रेशोल्ड मान प्राप्त या सेट करता है। डिफ़ॉल्ट मान 128. है

```csharp
public byte BinarizationThreshold { get; set; }
```

### उदाहरण

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

* class [ImageBinarizationOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../imagebinarizationoptions/)
* सभा [Aspose.Note](../../../)


