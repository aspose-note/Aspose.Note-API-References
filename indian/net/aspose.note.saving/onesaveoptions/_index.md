---
title: Class OneSaveOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.OneSaveOptions कक्ष. दस्तवेज़ क OneNote स्वरूप में सहेजते समय अतरक्त वकल्प नर्दष्ट करने देत है.
type: docs
weight: 810
url: /hi/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

दस्तावेज़ को OneNote स्वरूप में सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने देता है.

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | दस्तावेज़ सामग्री को एन्क्रिप्ट करने के लिए पासवर्ड प्राप्त करता है या सेट करता है. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | को सहेजते समय उपयोग किए जाने वाले फ़ॉन्ट की सेटिंग प्राप्त या सेट करता है |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | सहेजे जाने वाले पृष्ठों की संख्या प्राप्त करता है या सेट करता है। डिफ़ॉल्ट रूप से हैMaxValue जिसका मतलब है कि दस्तावेज़ के सभी पेज रेंडर किए जाएंगे. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | सहेजे जाने वाले पहले पृष्ठ की अनुक्रमणिका प्राप्त करता है या सेट करता है। डिफ़ॉल्ट रूप से 0. है |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | उस प्रारूप को प्राप्त करता है जिसमें दस्तावेज़ सहेजा गया है। |

### उदाहरण

दिखाता है कि एन्क्रिप्शन के साथ दस्तावेज़ को कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

दिखाता है कि OneSaveOptions का उपयोग करके किसी दस्तावेज़ को कैसे सहेजना है।

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### यह सभी देखें

* class [SaveOptions](../saveoptions/)
* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


