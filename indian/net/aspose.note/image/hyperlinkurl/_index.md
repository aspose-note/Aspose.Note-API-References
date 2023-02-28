---
title: Image.HyperlinkUrl
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Image संपत्त. छव से जुड़े हइपरलंक क प्रप्त य सेट करत है
type: docs
weight: 110
url: /hi/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

छवि से जुड़े हाइपरलिंक को प्राप्त या सेट करता है।

```csharp
public string HyperlinkUrl { get; set; }
```

### उदाहरण

दिखाता है कि हाइपरलिंक को इमेज से कैसे बाइंड किया जाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

### यह सभी देखें

* class [Image](../)
* नाम स्थान [Aspose.Note](../../image/)
* सभा [Aspose.Note](../../../)


