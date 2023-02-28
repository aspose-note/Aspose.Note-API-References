---
title: NumberList.FontColor
second_title: Aspose.Note für .NET-API-Referenz
description: NumberList eigendom. Ruft die Schriftfarbe ab oder legt sie fest.
type: docs
weight: 30
url: /de/net/aspose.note/numberlist/fontcolor/
---
## NumberList.FontColor property

Ruft die Schriftfarbe ab oder legt sie fest.

```csharp
public Color FontColor { get; set; }
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


