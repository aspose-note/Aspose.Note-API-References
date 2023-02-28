---
title: Style.IsBold
second_title: Aspose.Note for .NET API Reference
description: Style ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ του κειμένου είναι έντονη.
type: docs
weight: 60
url: /el/net/aspose.note/style/isbold/
---
## Style.IsBold property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το στυλ του κειμένου είναι έντονη.

```csharp
public bool IsBold { get; set; }
```

### Παραδείγματα

Ας τονίσουμε τους τίτλους της σελίδας μεταξύ άλλων κεφαλίδων αυξάνοντας το μέγεθος της γραμματοσειράς.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Επανάληψη στους τίτλους της σελίδας.
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

* class [Style](../)
* χώρος ονομάτων [Aspose.Note](../../style/)
* συνέλευση [Aspose.Note](../../../)


