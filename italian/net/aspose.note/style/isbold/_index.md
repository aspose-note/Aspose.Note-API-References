---
title: Style.IsBold
second_title: Aspose.Note per .NET API Reference
description: Style proprietà. Ottiene o imposta un valore che indica se lo stile del testo è in grassetto.
type: docs
weight: 60
url: /it/net/aspose.note/style/isbold/
---
## Style.IsBold property

Ottiene o imposta un valore che indica se lo stile del testo è in grassetto.

```csharp
public bool IsBold { get; set; }
```

### Esempi

Mettiamo in risalto i titoli delle pagine tra le altre intestazioni aumentando la dimensione del carattere.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Itera attraverso i titoli della pagina.
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

Sottolineiamo le ultime modifiche al testo evidenziando.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Ottieni i nodi RichText modificati la scorsa settimana.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Imposta il colore di evidenziazione
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Imposta il colore di evidenziazione
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

### Guarda anche

* class [Style](../)
* spazio dei nomi [Aspose.Note](../../style/)
* assemblea [Aspose.Note](../../../)


