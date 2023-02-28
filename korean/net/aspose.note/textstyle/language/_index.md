---
title: TextStyle.Language
second_title: .NET API 참조용 Aspose.Note
description: TextStyle 재산. 텍스트의 언어를 가져오거나 설정합니다.
type: docs
weight: 100
url: /ko/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

텍스트의 언어를 가져오거나 설정합니다.

```csharp
public CultureInfo Language { get; set; }
```

### 비고

보고InvariantCulture 속성이 설정되지 않은 경우.

### 예

텍스트의 교정 언어를 설정합니다.

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

### 또한보십시오

* class [TextStyle](../)
* 네임스페이스 [Aspose.Note](../../textstyle/)
* 집회 [Aspose.Note](../../../)


