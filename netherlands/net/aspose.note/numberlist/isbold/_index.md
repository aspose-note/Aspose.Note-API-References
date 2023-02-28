---
title: NumberList.IsBold
second_title: Aspose.Note voor .NET API-referentie
description: NumberList eigendom. Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl vet is.
type: docs
weight: 60
url: /nl/net/aspose.note/numberlist/isbold/
---
## NumberList.IsBold property

Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de tekststijl vet is.

```csharp
public bool IsBold { get; set; }
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


