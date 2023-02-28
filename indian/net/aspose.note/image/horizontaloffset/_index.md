---
title: Image.HorizontalOffset
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Image संपत्त. क्षैतज ऑफसेट प्रप्त य सेट करत है
type: docs
weight: 100
url: /hi/net/aspose.note/image/horizontaloffset/
---
## Image.HorizontalOffset property

क्षैतिज ऑफसेट प्राप्त या सेट करता है।

```csharp
public float HorizontalOffset { get; set; }
```

### उदाहरण

उपयोगकर्ता परिभाषित गुणों के साथ फ़ाइल से दस्तावेज़ में छवि जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// धारा से दस्तावेज़ लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

// दस्तावेज़ का पहला पृष्ठ प्राप्त करें।
Aspose.Note.Page page = doc.FirstChild;

// फ़ाइल से एक छवि लोड करें।
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // अपनी आवश्यकताओं के अनुसार छवि का आकार बदलें (वैकल्पिक)।
                              Width = 100,
                              Height = 100,

                              // पृष्ठ में छवि का स्थान सेट करें (वैकल्पिक)।
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // छवि संरेखण सेट करें
                              Alignment = HorizontalAlignment.Right
                          };

// छवि को पेज में जोड़ें।
page.AppendChildLast(image);
```

### यह सभी देखें

* class [Image](../)
* नाम स्थान [Aspose.Note](../../image/)
* सभा [Aspose.Note](../../../)


