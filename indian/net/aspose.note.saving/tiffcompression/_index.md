---
title: Enum TiffCompression
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.TiffCompression एनुम. नर्दष्ट करत है क दस्तवेज़ क TIFF प्ररूप में सहेजते समय कस प्रकर के संपड़न क उपयग करन है
type: docs
weight: 880
url: /hi/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

निर्दिष्ट करता है कि दस्तावेज़ को TIFF प्रारूप में सहेजते समय किस प्रकार के संपीड़न का उपयोग करना है।

```csharp
public enum TiffCompression
```

### मान

| नाम | कीमत | विवरण |
| --- | --- | --- |
| None | `1` | कोई संपीड़न निर्दिष्ट नहीं करता है। |
| Rle | `2` | आरएलई संपीड़न निर्दिष्ट करता है। |
| Ccitt3 | `3` | CCITT Group 3 फ़ैक्स एन्कोडिंग निर्दिष्ट करता है। |
| Ccitt4 | `4` | CCITT ग्रुप 4 फैक्स एन्कोडिंग निर्दिष्ट करता है। |
| Lzw | `5` | LZW संपीड़न निर्दिष्ट करता है। |
| PackBits | `32773` | Macintosh RLE संपीड़न निर्दिष्ट करता है। |
| Jpeg | `7` | जेपीईजी डीसीटी संपीड़न संपीड़न निर्दिष्ट करता है। |

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

* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


