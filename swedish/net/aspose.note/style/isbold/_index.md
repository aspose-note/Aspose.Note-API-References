---
title: Style.IsBold
second_title: Aspose.Note för .NET API-referens
description: Style fast egendom. Hämtar eller ställer in ett värde som anger om textstilen är fetstil.
type: docs
weight: 60
url: /sv/net/aspose.note/style/isbold/
---
## Style.IsBold property

Hämtar eller ställer in ett värde som anger om textstilen är fetstil.

```csharp
public bool IsBold { get; set; }
```

### Exempel

Låt oss betona sidans titlar bland andra rubriker genom att öka teckensnittets storlek.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Iterera genom sidans titlar.
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

Låt oss betona de senaste textens ändringar genom att markera.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Få RichText-noder modifierade förra veckan.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Ställ in högdagerfärg
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Ställ in högdagerfärg
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### Se även

* class [Style](../)
* namnutrymme [Aspose.Note](../../style/)
* hopsättning [Aspose.Note](../../../)


