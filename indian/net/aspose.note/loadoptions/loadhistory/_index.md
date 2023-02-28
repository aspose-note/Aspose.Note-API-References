---
title: LoadOptions.LoadHistory
second_title: Aspose.Note .NET API संदर्भ के लिए
description: LoadOptions संपत्त. एक मन प्रप्त य सेट करत है ज इंगत करत है क दस्तवेज़ लडर क इतहस क अनदेख करन चहए स्मृत और CPU उपयग क कम करने के लए इस वकल्प क उपयग करें डफ़ल्ट मन हैसत्य .
type: docs
weight: 30
url: /hi/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

एक मान प्राप्त या सेट करता है जो इंगित करता है कि दस्तावेज़ लोडर को इतिहास को अनदेखा करना चाहिए। स्मृति और CPU उपयोग को कम करने के लिए इस विकल्प का उपयोग करें। डिफ़ॉल्ट मान है`सत्य` .

```csharp
public bool LoadHistory { get; set; }
```

### उदाहरण

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

* class [LoadOptions](../)
* नाम स्थान [Aspose.Note](../../loadoptions/)
* सभा [Aspose.Note](../../../)


