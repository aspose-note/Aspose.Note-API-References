---
title: Interface INoteTag
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.INoteTag interfaccia. Linterfaccia per i tag delle note ovvero i tag non associati alle attività di Outlook.
type: docs
weight: 180
url: /it/net/aspose.note/inotetag/
---
## INoteTag interface

L'interfaccia per i tag delle note (ovvero i tag non associati alle attività di Outlook).

```csharp
public interface INoteTag : ITag
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | Ottiene o imposta il colore del carattere. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | Ottiene o imposta il colore di evidenziazione. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | Ottiene o imposta il testo dell'etichetta. |

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

* interface [ITag](../itag/)
* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


