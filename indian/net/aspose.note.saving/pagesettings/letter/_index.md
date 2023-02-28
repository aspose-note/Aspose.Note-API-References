---
title: PageSettings.Letter
second_title: Aspose.Note .NET API संदर्भ के लिए
description: PageSettings संपत्त. अक्षरप्ररूप पृष्ठ के लए सेटंग प्रप्त करत है.
type: docs
weight: 30
url: /hi/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

अक्षर-प्रारूप पृष्ठ के लिए सेटिंग प्राप्त करता है.

```csharp
public static PageSettings Letter { get; }
```

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

### यह सभी देखें

* class [PageSettings](../)
* नाम स्थान [Aspose.Note.Saving](../../pagesettings/)
* सभा [Aspose.Note](../../../)


