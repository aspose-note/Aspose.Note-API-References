---
title: ITag.Label
second_title: Aspose.Note per .NET API Reference
description: ITag proprietà. Ottiene il testo delletichetta.
type: docs
weight: 40
url: /it/net/aspose.note/itag/label/
---
## ITag.Label property

Ottiene il testo dell'etichetta.

```csharp
public string Label { get; }
```

### Esempi

Mostra come completare tutti gli elementi della casella di controllo relativi al "Progetto C".

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

Mostra come aprire tutti gli elementi della casella di controllo relativi al "Progetto C".

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Tags();

// Carica il documento in Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
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

* interface [ITag](../)
* spazio dei nomi [Aspose.Note](../../itag/)
* assemblea [Aspose.Note](../../../)


