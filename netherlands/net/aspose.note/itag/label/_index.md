---
title: ITag.Label
second_title: Aspose.Note voor .NET API-referentie
description: ITag eigendom. Haalt de labeltekst op.
type: docs
weight: 40
url: /nl/net/aspose.note/itag/label/
---
## ITag.Label property

Haalt de labeltekst op.

```csharp
public string Label { get; }
```

### Voorbeelden

Laat zien hoe u alle selectievakje-items met betrekking tot 'Project C' kunt voltooien.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
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

Laat zien hoe u alle selectievakje-items met betrekking tot 'Project C' kunt openen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
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

Laat zien hoe u toegang krijgt tot de details van een tag.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Tags();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Haal alle RichText-knooppunten op
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Doorloop elk knooppunt
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Eigenschappen ophalen
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

### Zie ook

* interface [ITag](../)
* naamruimte [Aspose.Note](../../itag/)
* montage [Aspose.Note](../../../)


