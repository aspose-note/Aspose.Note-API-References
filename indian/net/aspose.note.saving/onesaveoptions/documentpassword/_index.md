---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note .NET API संदर्भ के लिए
description: OneSaveOptions संपत्त. दस्तवेज़ समग्र क एन्क्रप्ट करने के लए पसवर्ड प्रप्त करत है य सेट करत है.
type: docs
weight: 20
url: /hi/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

दस्तावेज़ सामग्री को एन्क्रिप्ट करने के लिए पासवर्ड प्राप्त करता है या सेट करता है.

```csharp
public string DocumentPassword { get; set; }
```

### उदाहरण

दिखाता है कि एन्क्रिप्शन के साथ दस्तावेज़ को कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### यह सभी देखें

* class [OneSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../onesaveoptions/)
* सभा [Aspose.Note](../../../)


