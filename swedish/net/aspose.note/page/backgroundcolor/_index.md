---
title: Page.BackgroundColor
second_title: Aspose.Note för .NET API-referens
description: Page fast egendom. Hämtar eller ställer in sidans bakgrundsfärg.
type: docs
weight: 30
url: /sv/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

Hämtar eller ställer in sidans bakgrundsfärg.

```csharp
public Color BackgroundColor { get; set; }
```

### Exempel

Visar hur du ställer in sidans bakgrundsfärg.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Pages();

// Ladda OneNote-dokument och skaffa första barn           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

Visar hur man tillämpar mörkt temastil på ett dokument.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### Se även

* class [Page](../)
* namnutrymme [Aspose.Note](../../page/)
* hopsättning [Aspose.Note](../../../)


