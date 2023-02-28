---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note .NET API संदर्भ के लिए
description: LoadOptions संपत्त. एन्क्रप्टेड दस्तवेज़ समग्र के लए पसवर्ड प्रप्त य सेट करत है दस्तवेज़ पसवर्ड से सुरक्षत नहं हने क स्थत में मन क अनदेख कर दय जत है.
type: docs
weight: 20
url: /hi/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

एन्क्रिप्टेड दस्तावेज़ सामग्री के लिए पासवर्ड प्राप्त या सेट करता है। दस्तावेज़ पासवर्ड से सुरक्षित नहीं होने की स्थिति में मान को अनदेखा कर दिया जाता है.

```csharp
public string DocumentPassword { get; set; }
```

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

### यह सभी देखें

* class [LoadOptions](../)
* नाम स्थान [Aspose.Note](../../loadoptions/)
* सभा [Aspose.Note](../../../)


