---
title: Class NotebookLoadOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.NotebookLoadOptions कक्ष. नटबुक लड करने के लए उपयग कए जने वले वकल्प
type: docs
weight: 420
url: /hi/net/aspose.note/notebookloadoptions/
---
## NotebookLoadOptions class

नोटबुक लोड करने के लिए उपयोग किए जाने वाले विकल्प।

```csharp
public class NotebookLoadOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [NotebookLoadOptions](notebookloadoptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DeferredLoading](../../aspose.note/notebookloadoptions/deferredloading/) { get; set; } | यह इंगित करने वाला मान प्राप्त या सेट करता है कि क्या बच्चों के दस्तावेज़ को बाद में स्पष्ट रूप से लोड किया जाना चाहिए। |
| [InstantLoading](../../aspose.note/notebookloadoptions/instantloading/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि मूल दस्तावेज़ लोड होने पर बच्चों के दस्तावेज़ लोड किए जाने चाहिए या नहीं। |

### उदाहरण

एक एन्क्रिप्टेड नोटबुक को कैसे दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

### यह सभी देखें

* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


