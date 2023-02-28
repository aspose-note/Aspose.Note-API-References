---
title: Image.Tags
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Image संपत्त. अनुच्छेद के सभ टैग क सूच प्रप्त करत है
type: docs
weight: 160
url: /hi/net/aspose.note/image/tags/
---
## Image.Tags property

अनुच्छेद के सभी टैग की सूची प्राप्त करता है।

```csharp
public List<ITag> Tags { get; }
```

### उदाहरण

टैग के साथ नई छवि जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);

// छवि लोड करें
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// दस्तावेज़ नोड में छवि डालें
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// रूपरेखा तत्व नोड जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### यह सभी देखें

* interface [ITag](../../itag/)
* class [Image](../)
* नाम स्थान [Aspose.Note](../../image/)
* सभा [Aspose.Note](../../../)


