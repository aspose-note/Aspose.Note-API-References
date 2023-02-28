---
title: TextStyle.Language
second_title: Aspose.Note for .NET API リファレンス
description: TextStyle 財産. テキストの言語を取得または設定します
type: docs
weight: 100
url: /ja/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

テキストの言語を取得または設定します。

```csharp
public CultureInfo Language { get; set; }
```

### 備考

戻り値InvariantCultureプロパティが設定されていない場合。

### 例

テキストの校正言語を設定します。

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

### 関連項目

* class [TextStyle](../)
* 名前空間 [Aspose.Note](../../textstyle/)
* 組み立て [Aspose.Note](../../../)


