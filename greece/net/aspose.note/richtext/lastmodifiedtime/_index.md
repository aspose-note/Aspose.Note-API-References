---
title: RichText.LastModifiedTime
second_title: Aspose.Note for .NET API Reference
description: RichText ιδιοκτησία. Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.
type: docs
weight: 30
url: /el/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Παραδείγματα

Ας τονίσουμε τις τελευταίες αλλαγές του κειμένου επισημαίνοντας.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Λάβετε κόμβους εμπλουτισμένου κειμένου που τροποποιήθηκαν την περασμένη εβδομάδα.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Ορισμός χρώματος επισήμανσης
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Ορισμός χρώματος επισήμανσης
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### Δείτε επίσης

* class [RichText](../)
* χώρος ονομάτων [Aspose.Note](../../richtext/)
* συνέλευση [Aspose.Note](../../../)


