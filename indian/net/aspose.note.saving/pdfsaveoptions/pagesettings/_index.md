---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note .NET API संदर्भ के लिए
description: PdfSaveOptions संपत्त. दस्तवेज़ में प्रत्येक पृष्ठ के लए पृष्ठ सेटंग्स प्रप्त य सेट करत है डफ़ल्ट रूप से वर्तमन यूआईसल्चर पर नर्भर करत है  यूएस संस्कृतयं में अक्षर सेटंग हत है अन्य में ए 4 सेटंग्स हत हैं
type: docs
weight: 40
url: /hi/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

दस्तावेज़ में प्रत्येक पृष्ठ के लिए पृष्ठ सेटिंग्स प्राप्त या सेट करता है। डिफ़ॉल्ट रूप से वर्तमान यूआईसील्चर पर निर्भर करता है, * यूएस संस्कृतियों में अक्षर सेटिंग होती है, अन्य में ए 4 सेटिंग्स होती हैं।

```csharp
public PageSettings PageSettings { get; set; }
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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../pdfsaveoptions/)
* सभा [Aspose.Note](../../../)


