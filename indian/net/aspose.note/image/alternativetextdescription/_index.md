---
title: Image.AlternativeTextDescription
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Image संपत्त. छव के लए एक वैकल्पक टेक्स्ट प्रप्त करत है य सेट करत है
type: docs
weight: 30
url: /hi/net/aspose.note/image/alternativetextdescription/
---
## Image.AlternativeTextDescription property

छवि के लिए एक वैकल्पिक टेक्स्ट प्राप्त करता है या सेट करता है।

```csharp
public string AlternativeTextDescription { get; set; }
```

### उदाहरण

छवि के लिए टेक्स्ट विवरण सेट करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

### यह सभी देखें

* class [Image](../)
* नाम स्थान [Aspose.Note](../../image/)
* सभा [Aspose.Note](../../../)


