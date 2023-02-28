---
title: TextStyle.Language
second_title: Aspose.Note .NET API संदर्भ के लिए
description: TextStyle संपत्त. टेक्स्ट क भष प्रप्त य सेट करत है
type: docs
weight: 100
url: /hi/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

टेक्स्ट की भाषा प्राप्त या सेट करता है।

```csharp
public CultureInfo Language { get; set; }
```

### टिप्पणियों

रिटर्नInvariantCulture अगर संपत्ति सेट नहीं है।

### उदाहरण

टेक्स्ट के लिए अशुद्धि जाँच भाषा सेट करें।

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

### यह सभी देखें

* class [TextStyle](../)
* नाम स्थान [Aspose.Note](../../textstyle/)
* सभा [Aspose.Note](../../../)


