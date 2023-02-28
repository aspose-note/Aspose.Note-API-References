---
title: Page.BackgroundColor
second_title: Aspose.Note voor .NET API-referentie
description: Page eigendom. Hiermee wordt de achtergrondkleur van de pagina opgehaald of ingesteld.
type: docs
weight: 30
url: /nl/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

Hiermee wordt de achtergrondkleur van de pagina opgehaald of ingesteld.

```csharp
public Color BackgroundColor { get; set; }
```

### Voorbeelden

Laat zien hoe u de achtergrondkleur van de pagina instelt.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

Laat zien hoe u de donkere themastijl toepast op een document.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
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

### Zie ook

* class [Page](../)
* naamruimte [Aspose.Note](../../page/)
* montage [Aspose.Note](../../../)


