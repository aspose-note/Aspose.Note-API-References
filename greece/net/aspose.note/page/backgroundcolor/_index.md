---
title: Page.BackgroundColor
second_title: Aspose.Note for .NET API Reference
description: Page ιδιοκτησία. Λαμβάνει ή ορίζει το χρώμα φόντου της σελίδας.
type: docs
weight: 30
url: /el/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

Λαμβάνει ή ορίζει το χρώμα φόντου της σελίδας.

```csharp
public Color BackgroundColor { get; set; }
```

### Παραδείγματα

Δείχνει πώς να ορίσετε το χρώμα φόντου της σελίδας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Pages();

// Φορτώστε το έγγραφο του OneNote και αποκτήστε το πρώτο παιδί           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

Δείχνει πώς να εφαρμόσετε το στυλ σκούρου θέματος σε ένα έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
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

### Δείτε επίσης

* class [Page](../)
* χώρος ονομάτων [Aspose.Note](../../page/)
* συνέλευση [Aspose.Note](../../../)


