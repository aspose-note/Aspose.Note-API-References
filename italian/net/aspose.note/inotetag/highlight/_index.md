---
title: INoteTag.Highlight
second_title: Aspose.Note per .NET API Reference
description: INoteTag proprietà. Ottiene o imposta il colore di evidenziazione.
type: docs
weight: 20
url: /it/net/aspose.note/inotetag/highlight/
---
## INoteTag.Highlight property

Ottiene o imposta il colore di evidenziazione.

```csharp
public Color Highlight { get; set; }
```

### Esempi

Mostra come accedere ai dettagli di un tag.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Ottieni tutti i nodi RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Itera attraverso ogni nodo
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Recupera le proprietà
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
```

### Guarda anche

* interface [INoteTag](../)
* spazio dei nomi [Aspose.Note](../../inotetag/)
* assemblea [Aspose.Note](../../../)


