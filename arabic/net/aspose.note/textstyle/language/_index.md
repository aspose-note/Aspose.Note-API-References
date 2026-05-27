---
title: "TextStyle.Language"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية TextStyle. تحصل أو تعيّن لغة النص"
type: docs
weight: 100
url: /ar/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

يحصل أو يعيّن لغة النص.

```csharp
public CultureInfo Language { get; set; }
```

## ملاحظات

يرجع InvariantCulture إذا لم يتم تعيين الخاصية.

## أمثلة

تعيين لغة التدقيق لنص.

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

### انظر أيضًا

* class [TextStyle](../)
* namespace [Aspose.Note](../../textstyle/)
* assembly [Aspose.Note](../../../)


