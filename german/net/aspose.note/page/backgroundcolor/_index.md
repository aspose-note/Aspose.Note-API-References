---
title: Page.BackgroundColor
second_title: Aspose.Note für .NET-API-Referenz
description: Page eigendom. Ruft die Hintergrundfarbe der Seite ab oder legt sie fest.
type: docs
weight: 30
url: /de/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

Ruft die Hintergrundfarbe der Seite ab oder legt sie fest.

```csharp
public Color BackgroundColor { get; set; }
```

### Beispiele

Zeigt, wie die Hintergrundfarbe der Seite festgelegt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden und erstes untergeordnetes Element abrufen           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

Zeigt, wie man den dunklen Designstil auf ein Dokument anwendet.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
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

### Siehe auch

* class [Page](../)
* namensraum [Aspose.Note](../../page/)
* Montage [Aspose.Note](../../../)


