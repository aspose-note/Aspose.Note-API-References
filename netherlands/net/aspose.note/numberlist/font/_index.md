---
title: NumberList.Font
second_title: Aspose.Note voor .NET API-referentie
description: NumberList eigendom. Haalt de naam van het lettertype op of stelt deze in.
type: docs
weight: 20
url: /nl/net/aspose.note/numberlist/font/
---
## NumberList.Font property

Haalt de naam van het lettertype op of stelt deze in.

```csharp
public string Font { get; set; }
```

### Voorbeelden

Laat zien hoe informatie over de opmaak van de lijst kan worden opgehaald.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Haal een verzameling knooppunten van het overzichtselement op
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Doorloop elk knooppunt
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Lettertypenaam ophalen
        Console.WriteLine("Font Name: " + list.Font);

        // Letterlengte ophalen
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Lettergrootte ophalen
        Console.WriteLine("Font Size: " + list.FontSize);

        // Letterkleur ophalen
        Console.WriteLine("Font Color: " + list.FontColor);

        // Formaat ophalen
        Console.WriteLine("Font format: " + list.Format);

        // Vink vet aan
        Console.WriteLine("Is bold: " + list.IsBold);

        // Controleer cursief
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### Zie ook

* class [NumberList](../)
* naamruimte [Aspose.Note](../../numberlist/)
* montage [Aspose.Note](../../../)


