---
title: Page.BackgroundColor
second_title: Aspose.Note per .NET API Reference
description: Page proprietà. Ottiene o imposta il colore di sfondo della pagina.
type: docs
weight: 30
url: /it/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

Ottiene o imposta il colore di sfondo della pagina.

```csharp
public Color BackgroundColor { get; set; }
```

### Esempi

Mostra come impostare il colore di sfondo della pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote e ottieni il primo figlio           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

Mostra come applicare lo stile del tema scuro a un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
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

### Guarda anche

* class [Page](../)
* spazio dei nomi [Aspose.Note](../../page/)
* assemblea [Aspose.Note](../../../)


