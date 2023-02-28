---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note .NET API संदर्भ के लिए
description: DocumentFontsSubsystem तरक. डफ़ल्ट के रूप में नर्दष्ट स्ट्रम से फ़न्ट क उपयग करके नय दस्तवेज़फ़न्टसबसस्टम उदहरण बनएं
type: docs
weight: 50
url: /hi/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

डिफ़ॉल्ट के रूप में निर्दिष्ट स्ट्रीम से फ़ॉन्ट का उपयोग करके नया दस्तावेज़फ़ॉन्टसबसिस्टम उदाहरण बनाएं।

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| defaultFontStream | Stream | डिफ़ॉल्ट फ़ॉन्ट नाम वाली स्ट्रीम. |
| fontsSubstitutions | Dictionary`2 | फोंट प्रतिस्थापन। |

### प्रतिलाभ की मात्रा

द[`DocumentFontsSubsystem`](../) .

### उदाहरण

दिखाता है कि स्ट्रीम से डिफ़ॉल्ट फ़ॉन्ट का उपयोग करके किसी दस्तावेज़ को पीडीएफ प्रारूप में कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// दस्तावेज़ को पीडीएफ के रूप में सहेजें
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### यह सभी देखें

* class [DocumentFontsSubsystem](../)
* नाम स्थान [Aspose.Note.Fonts](../../documentfontssubsystem/)
* सभा [Aspose.Note](../../../)


