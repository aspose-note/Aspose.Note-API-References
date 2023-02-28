---
title: Page.Clone
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Page तरक. पेज क क्लन करत है
type: docs
weight: 140
url: /hi/net/aspose.note/page/clone/
---
## Page.Clone method

पेज को क्लोन करता है।

```csharp
public Page Clone(bool cloneHistory = false)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| cloneHistory | Boolean | निर्दिष्ट करता है कि पृष्ठ का इतिहास क्लोन किया जाना चाहिए या नहीं... |

### प्रतिलाभ की मात्रा

पृष्ठ का एक क्लोन।

### उदाहरण

दिखाता है कि किसी पृष्ठ के वर्तमान संस्करण को इतिहास में कैसे पुश करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें और पहला बच्चा प्राप्त करें           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

पेज को क्लोन करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// इतिहास के बिना नए दस्तावेज़ में क्लोन करें
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// इतिहास के साथ नए दस्तावेज़ में क्लोन करें
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### यह सभी देखें

* class [Page](../)
* नाम स्थान [Aspose.Note](../../page/)
* सभा [Aspose.Note](../../../)


