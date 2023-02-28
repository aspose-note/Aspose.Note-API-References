---
title: RichText.LastModifiedTime
second_title: Aspose.Note für .NET-API-Referenz
description: RichText eigendom. Ruft die letzte Änderungszeit ab oder setzt sie.
type: docs
weight: 30
url: /de/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

Ruft die letzte Änderungszeit ab oder setzt sie.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Beispiele

Lassen Sie uns die Änderungen des letzten Textes hervorheben, indem wir sie hervorheben.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// RichText-Knoten abrufen, die letzte Woche geändert wurden.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Hervorhebungsfarbe setzen
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Hervorhebungsfarbe setzen
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### Siehe auch

* class [RichText](../)
* namensraum [Aspose.Note](../../richtext/)
* Montage [Aspose.Note](../../../)


