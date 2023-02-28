---
title: NumberList.Format
second_title: Aspose.Note für .NET-API-Referenz
description: NumberList eigendom. Holt oder setzt das Format des Zeilenkopfes. Für Listen mit Aufzählungszeichen steht ein Aufzählungszeichen.
type: docs
weight: 50
url: /de/net/aspose.note/numberlist/format/
---
## NumberList.Format property

Holt oder setzt das Format des Zeilenkopfes. Für Listen mit Aufzählungszeichen steht ein Aufzählungszeichen.

```csharp
public string Format { get; set; }
```

### Beispiele

Zeigt, wie Informationen zur Formatierung von Listen abgerufen werden.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Sammlungsknoten des Gliederungselements abrufen
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Durch jeden Knoten iterieren
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Schriftartnamen abrufen
        Console.WriteLine("Font Name: " + list.Font);

        // Schriftlänge abrufen
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Schriftgröße abrufen
        Console.WriteLine("Font Size: " + list.FontSize);

        // Schriftfarbe abrufen
        Console.WriteLine("Font Color: " + list.FontColor);

        // Format abrufen
        Console.WriteLine("Font format: " + list.Format);

        // Fett markieren
        Console.WriteLine("Is bold: " + list.IsBold);

        // Kursiv prüfen
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### Siehe auch

* class [NumberList](../)
* namensraum [Aspose.Note](../../numberlist/)
* Montage [Aspose.Note](../../../)


