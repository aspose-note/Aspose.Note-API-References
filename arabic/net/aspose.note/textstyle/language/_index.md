---
title: TextStyle.Language
second_title: Aspose.Note لمرجع NET API
description: TextStyle ملكية. الحصول على لغة النص أو تحديدها .
type: docs
weight: 100
url: /ar/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

الحصول على لغة النص أو تحديدها .

```csharp
public CultureInfo Language { get; set; }
```

### ملاحظات

عائداتInvariantCulture إذا لم يتم تعيين الخاصية.

### أمثلة

تعيين لغة التدقيق للنص.

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

### أنظر أيضا

* class [TextStyle](../)
* مساحة الاسم [Aspose.Note](../../textstyle/)
* المجسم [Aspose.Note](../../../)


