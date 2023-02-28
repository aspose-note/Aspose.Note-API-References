---
title: TextStyle.Language
second_title: Aspose.Note for .NET API 参考
description: TextStyle 财产. 获取或设置文本的语言
type: docs
weight: 100
url: /zh/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

获取或设置文本的语言。

```csharp
public CultureInfo Language { get; set; }
```

### 评论

退货InvariantCulture如果未设置该属性。

### 例子

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

### 也可以看看

* class [TextStyle](../)
* 命名空间 [Aspose.Note](../../textstyle/)
* 部件 [Aspose.Note](../../../)


