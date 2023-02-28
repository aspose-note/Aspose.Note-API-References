---
title: RichText.LastModifiedTime
second_title: Aspose.Note per .NET API Reference
description: RichText proprietà. Ottiene o imposta lora dellultima modifica.
type: docs
weight: 30
url: /it/net/aspose.note/richtext/lastmodifiedtime/
---
## RichText.LastModifiedTime property

Ottiene o imposta l'ora dell'ultima modifica.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Esempi

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

* class [RichText](../)
* spazio dei nomi [Aspose.Note](../../richtext/)
* assemblea [Aspose.Note](../../../)


