---
title: Interface INoteTag
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.INoteTag koppel. Die Schnittstelle für NotizTags dh Tags die nicht mit OutlookAufgaben verknüpft sind.
type: docs
weight: 180
url: /de/net/aspose.note/inotetag/
---
## INoteTag interface

Die Schnittstelle für Notiz-Tags (dh Tags, die nicht mit Outlook-Aufgaben verknüpft sind).

```csharp
public interface INoteTag : ITag
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | Ruft die Schriftfarbe ab oder legt sie fest. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | Ruft die Hervorhebungsfarbe ab oder legt sie fest. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | Ruft den Beschriftungstext ab oder legt ihn fest. |

### Beispiele

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

* interface [ITag](../itag/)
* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


