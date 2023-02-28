---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note .NET API संदर्भ के लिए
description: DocumentFontsSubsystem तरक. डफ़ल्ट के रूप में नर्दष्ट फ़इल से फ़न्ट क उपयग करके नय दस्तवेज़फ़न्टसबसस्टम उदहरण बनएं
type: docs
weight: 40
url: /hi/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

डिफ़ॉल्ट के रूप में निर्दिष्ट फ़ाइल से फ़ॉन्ट का उपयोग करके नया दस्तावेज़फ़ॉन्टसबसिस्टम उदाहरण बनाएं।

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | डिफ़ॉल्ट फ़ॉन्ट नाम वाली फ़ाइल. |
| fontsSubstitutions | Dictionary`2 | फोंट प्रतिस्थापन। |

### प्रतिलाभ की मात्रा

द[`DocumentFontsSubsystem`](../) .

### उदाहरण

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

### यह सभी देखें

* class [DocumentFontsSubsystem](../)
* नाम स्थान [Aspose.Note.Fonts](../../documentfontssubsystem/)
* सभा [Aspose.Note](../../../)


