---
title: TextStyle.Language
second_title: Aspose.Note for .NET API Reference
description: TextStyle property. Gets or sets the language of the text
type: docs
weight: 100
url: /net/aspose.note/textstyle/language/
---
## TextStyle.Language property

Gets or sets the language of the text.

```csharp
public CultureInfo Language { get; set; }
```

## Remarks

Returns InvariantCulture if the property is not set.

## Examples

Set proofing language for a text.

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

### See Also

* class [TextStyle](../)
* namespace [Aspose.Note](../../textstyle/)
* assembly [Aspose.Note](../../../)


