---
title: RichText.LastModifiedTime
second_title: Aspose.Note voor .NET API-referentie
description: RichText eigendom. Haalt of stelt de laatst gewijzigde tijd in.
type: docs
weight: 30
url: /nl/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

Haalt of stelt de laatst gewijzigde tijd in.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Voorbeelden

Laten we de wijzigingen in de laatste tekst benadrukken door te markeren.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Ontvang RichText-knooppunten die vorige week zijn gewijzigd.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Markeringskleur instellen
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Markeringskleur instellen
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### Zie ook

* class [RichText](../)
* naamruimte [Aspose.Note](../../richtext/)
* montage [Aspose.Note](../../../)


