---
title: Style.IsBold
second_title: Aspose.Note voor .NET API-referentie
description: Style eigendom. Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl vet is.
type: docs
weight: 60
url: /nl/net/aspose.note/style/isbold/
---
## Style.IsBold property

Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl vet is.

```csharp
public bool IsBold { get; set; }
```

### Voorbeelden

Laten we de titels van de pagina onder andere kopteksten benadrukken door de lettergrootte te vergroten.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Herhaal de paginatitels.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

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

* class [Style](../)
* naamruimte [Aspose.Note](../../style/)
* montage [Aspose.Note](../../../)


