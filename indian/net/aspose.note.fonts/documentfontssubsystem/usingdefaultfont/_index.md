---
title: DocumentFontsSubsystem.UsingDefaultFont
second_title: Aspose.Note .NET API संदर्भ के लिए
description: DocumentFontsSubsystem तरक. नर्दष्ट डफ़ल्ट फ़न्ट नम क उपयग करके नय दस्तवेज़फ़न्टसबसस्टम उदहरण बनएँ
type: docs
weight: 30
url: /hi/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

निर्दिष्ट डिफ़ॉल्ट फ़ॉन्ट नाम का उपयोग करके नया दस्तावेज़फ़ॉन्टसबसिस्टम उदाहरण बनाएँ।

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| defaultFontName | String | डिफ़ॉल्ट फ़ॉन्ट नाम. |
| fontsSubstitutions | Dictionary`2 | फोंट प्रतिस्थापन। |

### प्रतिलाभ की मात्रा

द[`DocumentFontsSubsystem`](../) .

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

### यह सभी देखें

* class [DocumentFontsSubsystem](../)
* नाम स्थान [Aspose.Note.Fonts](../../documentfontssubsystem/)
* सभा [Aspose.Note](../../../)


