---
title: ITag.Status
second_title: Aspose.Note per .NET API Reference
description: ITag proprietà. Ottiene o imposta lo stato.
type: docs
weight: 50
url: /it/net/aspose.note/itag/status/
---
## ITag.Status property

Ottiene o imposta lo stato.

```csharp
public TagStatus Status { get; }
```

### Valore della proprietà

Il[`TagStatus`](../../tagstatus/) .

### Esempi

Mostra come accedere ai dettagli delle attività di Outlook.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tasks();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni tutti i nodi RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Itera attraverso ogni nodo
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Recupera le proprietà
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

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

* enum [TagStatus](../../tagstatus/)
* interface [ITag](../)
* spazio dei nomi [Aspose.Note](../../itag/)
* assemblea [Aspose.Note](../../../)


