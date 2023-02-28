---
title: TextStyle.Language
second_title: Aspose.Note untuk Referensi .NET API
description: TextStyle Properti. Mendapat atau menyetel bahasa teks.
type: docs
weight: 100
url: /id/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

Mendapat atau menyetel bahasa teks.

```csharp
public CultureInfo Language { get; set; }
```

### Perkataan

PengembalianInvariantCulture jika properti tidak diatur.

### Contoh

Atur bahasa pemeriksaan untuk teks.

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

### Lihat juga

* class [TextStyle](../)
* ruang nama [Aspose.Note](../../textstyle/)
* perakitan [Aspose.Note](../../../)


