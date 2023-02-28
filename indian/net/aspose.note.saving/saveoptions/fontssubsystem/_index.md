---
title: SaveOptions.FontsSubsystem
second_title: Aspose.Note .NET API संदर्भ के लिए
description: SaveOptions संपत्त. क सहेजते समय उपयग कए जने वले फ़न्ट क सेटंग प्रप्त य सेट करत है
type: docs
weight: 10
url: /hi/net/aspose.note.saving/saveoptions/fontssubsystem/
---
## SaveOptions.FontsSubsystem property

को सहेजते समय उपयोग किए जाने वाले फ़ॉन्ट की सेटिंग प्राप्त या सेट करता है

```csharp
public FontsSubsystem FontsSubsystem { get; set; }
```

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

* class [FontsSubsystem](../../../aspose.note.fonts/fontssubsystem/)
* class [SaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../saveoptions/)
* सभा [Aspose.Note](../../../)


