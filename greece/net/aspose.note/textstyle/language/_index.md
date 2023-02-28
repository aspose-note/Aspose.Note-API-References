---
title: TextStyle.Language
second_title: Aspose.Note for .NET API Reference
description: TextStyle ιδιοκτησία. Λαμβάνει ή ορίζει τη γλώσσα του κειμένου.
type: docs
weight: 100
url: /el/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

Λαμβάνει ή ορίζει τη γλώσσα του κειμένου.

```csharp
public CultureInfo Language { get; set; }
```

### Παρατηρήσεις

ΕπιστροφέςInvariantCulture εάν το ακίνητο δεν έχει οριστεί.

### Παραδείγματα

Ορισμός γλώσσας διόρθωσης για ένα κείμενο.

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

### Δείτε επίσης

* class [TextStyle](../)
* χώρος ονομάτων [Aspose.Note](../../textstyle/)
* συνέλευση [Aspose.Note](../../../)


