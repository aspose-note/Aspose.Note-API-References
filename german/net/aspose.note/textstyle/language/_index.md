---
title: TextStyle.Language
second_title: Aspose.Note für .NET-API-Referenz
description: TextStyle eigendom. Holt oder setzt die Sprache des Textes.
type: docs
weight: 100
url: /de/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

Holt oder setzt die Sprache des Textes.

```csharp
public CultureInfo Language { get; set; }
```

### Bemerkungen

Kehrt zurückInvariantCulture wenn die Eigenschaft nicht gesetzt ist.

### Beispiele

Legen Sie die Korrektursprache für einen Text fest.

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

### Siehe auch

* class [TextStyle](../)
* namensraum [Aspose.Note](../../textstyle/)
* Montage [Aspose.Note](../../../)


