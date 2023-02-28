---
title: ImageSaveOptions.TiffCompression
second_title: Aspose.Note .NET API संदर्भ के लिए
description: ImageSaveOptions संपत्त. टआईएफएफ प्ररूप में जेनरेट क गई छवयं क सहेजते समय उपयग करने के लए संपड़न के प्रकर क प्रप्त य सेट करत है
type: docs
weight: 60
url: /hi/net/aspose.note.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

टीआईएफएफ प्रारूप में जेनरेट की गई छवियों को सहेजते समय उपयोग करने के लिए संपीड़न के प्रकार को प्राप्त या सेट करता है।

```csharp
public TiffCompression TiffCompression { get; set; }
```

### उदाहरण

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

### यह सभी देखें

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../imagesaveoptions/)
* सभा [Aspose.Note](../../../)


