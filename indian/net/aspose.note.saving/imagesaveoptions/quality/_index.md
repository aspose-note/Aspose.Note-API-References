---
title: ImageSaveOptions.Quality
second_title: Aspose.Note .NET API संदर्भ के लिए
description: ImageSaveOptions संपत्त. सहेज गई छव क गुणवत्त नर्धरत करने वल मन प्रप्त य सेट करत है
type: docs
weight: 40
url: /hi/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

सहेजी गई छवि की गुणवत्ता निर्धारित करने वाला मान प्राप्त या सेट करता है।

```csharp
public int Quality { get; set; }
```

### टिप्पणियों

गुणवत्ता श्रेणी के लिए उपयोगी मानों की सीमा 0 से 100 तक है। निर्दिष्ट संख्या जितनी कम होगी, संपीड़न उतना ही अधिक होगा और इसलिए छवि की गुणवत्ता कम होगी। शून्य आपको सबसे कम गुणवत्ता वाली छवि देगा और 100 उच्चतम . डिफ़ॉल्ट मान 90. है

### उदाहरण

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

### यह सभी देखें

* class [ImageSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../imagesaveoptions/)
* सभा [Aspose.Note](../../../)


