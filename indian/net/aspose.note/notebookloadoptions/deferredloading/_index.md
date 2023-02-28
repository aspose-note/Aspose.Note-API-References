---
title: NotebookLoadOptions.DeferredLoading
second_title: Aspose.Note .NET API संदर्भ के लिए
description: NotebookLoadOptions संपत्त. यह इंगत करने वल मन प्रप्त य सेट करत है क क्य बच्चं के दस्तवेज़ क बद में स्पष्ट रूप से लड कय जन चहए
type: docs
weight: 20
url: /hi/net/aspose.note/notebookloadoptions/deferredloading/
---
## NotebookLoadOptions.DeferredLoading property

यह इंगित करने वाला मान प्राप्त या सेट करता है कि क्या बच्चों के दस्तावेज़ को बाद में स्पष्ट रूप से लोड किया जाना चाहिए।

```csharp
public bool DeferredLoading { get; set; }
```

### टिप्पणियों

डिफ़ॉल्ट मान है`असत्य` , इसलिए चाइल्ड दस्तावेज़ निहित रूप से लोड किए जाएंगे. मान`सत्य` संकेत दे रहा है कि उपयोगकर्ता को कॉल करना चाहिए[`LoadChildDocument`](../../notebook/loadchilddocument/) या नोटबुक के स्वयं लोड होने के बाद प्रत्येक नोटबुक के चाइल्ड नोड के लिए. यदि मान है`सत्य` ,[`InstantLoading`](../instantloading/) विकल्प पर ध्यान नहीं दिया जाएगा. यदि नोटबुक स्ट्रीम से लोड हो रहा है, तो मान हमेशा होता है`सत्य` बावजूद उपयोगकर्ता द्वारा स्पष्ट रूप से सेट किया गया था`असत्य` .

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

* class [NotebookLoadOptions](../)
* नाम स्थान [Aspose.Note](../../notebookloadoptions/)
* सभा [Aspose.Note](../../../)


