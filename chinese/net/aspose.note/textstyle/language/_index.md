---
title: "TextStyle.Language"
second_title: "Aspose.Note for .NET API 参考"
description: "TextStyle 属性。获取或设置文本的语言"
type: docs
weight: 100
url: /zh/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

获取或设置文本的语言。

```csharp
public CultureInfo Language { get; set; }
```

## 备注

如果属性未设置，则返回 InvariantCulture。

## 示例

为文本设置校对语言。

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

### 另请参阅

* class [TextStyle](../)
* namespace [Aspose.Note](../../textstyle/)
* assembly [Aspose.Note](../../../)


