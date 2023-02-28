---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Fonts.DocumentFontsSubsystem कक्ष. Aspose.Note.Fonts.FontsSubsystem क सरल कर्यन्वयन retrievesFontFamily OS. से वस्तु
type: docs
weight: 100
url: /hi/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Aspose.Note.Fonts.FontsSubsystem का सरल कार्यान्वयन। retrievesFontFamily OS. से वस्तु

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | का एक नया उदाहरण प्रारंभ करता है`DocumentFontsSubsystem` वर्ग. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | का एक नया उदाहरण प्रारंभ करता है`DocumentFontsSubsystem` वर्ग. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | का एक नया उदाहरण प्रारंभ करता है`DocumentFontsSubsystem` वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | स्थिर डिफ़ॉल्ट उदाहरण प्राप्त या सेट करता है। |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | डिफ़ॉल्ट फ़ॉन्ट प्राप्त या सेट करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | निर्दिष्ट डिफ़ॉल्ट फ़ॉन्ट नाम का उपयोग करके नया दस्तावेज़फ़ॉन्टसबसिस्टम उदाहरण बनाएँ। |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | डिफ़ॉल्ट के रूप में निर्दिष्ट फ़ाइल से फ़ॉन्ट का उपयोग करके नया दस्तावेज़फ़ॉन्टसबसिस्टम उदाहरण बनाएं। |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | डिफ़ॉल्ट के रूप में निर्दिष्ट स्ट्रीम से फ़ॉन्ट का उपयोग करके नया दस्तावेज़फ़ॉन्टसबसिस्टम उदाहरण बनाएं। |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | फ़ॉन्ट जोड़ें. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | फ़ॉन्ट जोड़ें. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | फ़ॉन्ट जोड़ें. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | फ़ॉन्ट प्रतिस्थापन जोड़ता है। |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | फ़ॉन्ट परिवार हो जाता है। |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | सभी ट्रू टाइप फ़ॉन्ट निर्दिष्ट फ़ोल्डर से आंतरिक संग्रह में लोड करता है। |

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

* class [FontsSubsystem](../fontssubsystem/)
* नाम स्थान [Aspose.Note.Fonts](../../aspose.note.fonts/)
* सभा [Aspose.Note](../../)


