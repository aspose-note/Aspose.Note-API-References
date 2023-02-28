---
title: Enum BinarizationMethod
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.BinarizationMethod एनुम. एक छव के लए बनरइजेशन वध नर्दष्ट करत है
type: docs
weight: 560
url: /hi/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

एक छवि के लिए बिनराइजेशन विधि निर्दिष्ट करता है।

```csharp
public enum BinarizationMethod
```

### मान

| नाम | कीमत | विवरण |
| --- | --- | --- |
| FixedThreshold | `0` | छवि का द्वैतकरण निर्दिष्ट निश्चित सीमा का उपयोग करके किया जाता है। |
| Otsu | `1` | दहलीज का मूल्यांकन करने के लिए ओत्सु की विधि का उपयोग करके छवि का द्वैतकरण अनुकूल रूप से किया जाता है। |

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


