---
title: ITag.Status
second_title: Aspose.Note für .NET-API-Referenz
description: ITag eigendom. Ruft den Status ab oder setzt ihn.
type: docs
weight: 50
url: /de/net/aspose.note/itag/status/
---
## ITag.Status property

Ruft den Status ab oder setzt ihn.

```csharp
public TagStatus Status { get; }
```

### Eigentumswert

Die[`TagStatus`](../../tagstatus/) .

### Beispiele

Zeigt, wie auf Details der Outlook-Aufgaben zugegriffen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tasks();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Alle RichText-Knoten abrufen
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Durch jeden Knoten iterieren
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Eigenschaften abrufen
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

Zeigt, wie auf die Details eines Tags zugegriffen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Tags();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Alle RichText-Knoten abrufen
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Durch jeden Knoten iterieren
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Eigenschaften abrufen
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

### Siehe auch

* enum [TagStatus](../../tagstatus/)
* interface [ITag](../)
* namensraum [Aspose.Note](../../itag/)
* Montage [Aspose.Note](../../../)


