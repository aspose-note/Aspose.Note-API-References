---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note .NET API संदर्भ के लिए
description: PageSettings संपत्त. असमत ऊंचई वले ए4प्ररूप पृष्ठ के लए सेटंग प्रप्त करत है.
type: docs
weight: 20
url: /hi/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

असीमित ऊंचाई वाले ए4-प्रारूप पृष्ठ के लिए सेटिंग प्राप्त करता है.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### उदाहरण

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

* class [PageSettings](../)
* नाम स्थान [Aspose.Note.Saving](../../pagesettings/)
* सभा [Aspose.Note](../../../)


