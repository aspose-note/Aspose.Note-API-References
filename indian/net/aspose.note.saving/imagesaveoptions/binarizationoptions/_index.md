---
title: ImageSaveOptions.BinarizationOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: ImageSaveOptions संपत्त. छव के द्वैतकरण के लए वकल्प प्रप्त य सेट करत है
type: docs
weight: 20
url: /hi/net/aspose.note.saving/imagesaveoptions/binarizationoptions/
---
## ImageSaveOptions.BinarizationOptions property

छवि के द्वैतकरण के लिए विकल्प प्राप्त या सेट करता है।

```csharp
public ImageBinarizationOptions BinarizationOptions { get; set; }
```

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

* class [ImageBinarizationOptions](../../imagebinarizationoptions/)
* class [ImageSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../imagesaveoptions/)
* सभा [Aspose.Note](../../../)


