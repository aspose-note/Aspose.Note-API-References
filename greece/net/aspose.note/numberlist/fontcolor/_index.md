---
title: NumberList.FontColor
second_title: Aspose.Note for .NET API Reference
description: NumberList ιδιοκτησία. Παίρνει ή ορίζει το χρώμα της γραμματοσειράς.
type: docs
weight: 30
url: /el/net/aspose.note/numberlist/fontcolor/
---
## NumberList.FontColor property

Παίρνει ή ορίζει το χρώμα της γραμματοσειράς.

```csharp
public Color FontColor { get; set; }
```

### Παραδείγματα

Δείχνει πώς να ανακτήσετε πληροφορίες σχετικά με τη μορφοποίηση της λίστας.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Ανακτήστε έναν κόμβο συλλογής του στοιχείου περιγράμματος
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Επανάληψη σε κάθε κόμβο
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Ανάκτηση ονόματος γραμματοσειράς
        Console.WriteLine("Font Name: " + list.Font);

        // Ανάκτηση μήκους γραμματοσειράς
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Ανάκτηση μεγέθους γραμματοσειράς
        Console.WriteLine("Font Size: " + list.FontSize);

        // Ανάκτηση χρώματος γραμματοσειράς
        Console.WriteLine("Font Color: " + list.FontColor);

        // Ανάκτηση μορφής
        Console.WriteLine("Font format: " + list.Format);

        // Επιλέξτε έντονη γραφή
        Console.WriteLine("Is bold: " + list.IsBold);

        // Έλεγχος πλάγιας γραφής
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### Δείτε επίσης

* class [NumberList](../)
* χώρος ονομάτων [Aspose.Note](../../numberlist/)
* συνέλευση [Aspose.Note](../../../)


