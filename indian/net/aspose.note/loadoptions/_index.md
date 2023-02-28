---
title: Class LoadOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.LoadOptions कक्ष. दस्तवेज़ लड करने के लए उपयग कए जने वले वकल्प
type: docs
weight: 320
url: /hi/net/aspose.note/loadoptions/
---
## LoadOptions class

दस्तावेज़ लोड करने के लिए उपयोग किए जाने वाले विकल्प।

```csharp
public class LoadOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [LoadOptions](loadoptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | एन्क्रिप्टेड दस्तावेज़ सामग्री के लिए पासवर्ड प्राप्त या सेट करता है। दस्तावेज़ पासवर्ड से सुरक्षित नहीं होने की स्थिति में मान को अनदेखा कर दिया जाता है. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि दस्तावेज़ लोडर को इतिहास को अनदेखा करना चाहिए। स्मृति और CPU उपयोग को कम करने के लिए इस विकल्प का उपयोग करें। डिफ़ॉल्ट मान है`सत्य` . |

### उदाहरण

एक एन्क्रिप्टेड दस्तावेज़ को कैसे दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

एक एन्क्रिप्टेड नोटबुक को कैसे दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

दिखाता है कि पृष्ठ का इतिहास कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// पहला पेज प्राप्त करें
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### यह सभी देखें

* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


