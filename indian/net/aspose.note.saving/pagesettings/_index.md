---
title: Class PageSettings
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.PageSettings कक्ष. पृष्ठ के लए लेआउट सेटंग्स क प्रतनधत्व करत है
type: docs
weight: 820
url: /hi/net/aspose.note.saving/pagesettings/
---
## PageSettings class

पृष्ठ के लिए लेआउट सेटिंग्स का प्रतिनिधित्व करता है।

```csharp
public class PageSettings
```

## गुण

| नाम | विवरण |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | A4-प्रारूप पृष्ठ के लिए सेटिंग प्राप्त करता है. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | असीमित ऊंचाई वाले ए4-प्रारूप पृष्ठ के लिए सेटिंग प्राप्त करता है. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | अक्षर-प्रारूप पृष्ठ के लिए सेटिंग प्राप्त करता है. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | असीमित ऊंचाई वाले अक्षर-प्रारूप पृष्ठ के लिए सेटिंग प्राप्त करता है. |

### उदाहरण

लेटर पेज लेआउट के साथ पीडीएफ प्रारूप में दस्तावेज़ को कैसे सहेजना है, दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// दस्तावेज़ को सहेजें।
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

दिखाता है कि ऊंचाई सीमा के बिना A4 पेज लेआउट के साथ पीडीएफ प्रारूप में दस्तावेज़ को कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// दस्तावेज़ को सहेजें।
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### यह सभी देखें

* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


