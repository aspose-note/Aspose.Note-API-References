---
title: TextStyle.Language
second_title: Aspose.Note voor .NET API-referentie
description: TextStyle eigendom. Haalt de taal van de tekst op of stelt deze in.
type: docs
weight: 100
url: /nl/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

Haalt de taal van de tekst op of stelt deze in.

```csharp
public CultureInfo Language { get; set; }
```

### Opmerkingen

Geeft terugInvariantCulture als de eigenschap niet is ingesteld.

### Voorbeelden

Taal voor proeflezen instellen voor een tekst.

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

### Zie ook

* class [TextStyle](../)
* naamruimte [Aspose.Note](../../textstyle/)
* montage [Aspose.Note](../../../)


