---
title: NumberList.IsItalic
second_title: Aspose.Note för .NET API-referens
description: NumberList fast egendom. Hämtar eller ställer in ett värde som anger om textstilen är kursiv.
type: docs
weight: 70
url: /sv/net/aspose.note/numberlist/isitalic/
---
## NumberList.IsItalic property

Hämtar eller ställer in ett värde som anger om textstilen är kursiv.

```csharp
public bool IsItalic { get; set; }
```

### Exempel

Visar hur man hämtar information om listans formatering.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Hämta en samling noder av konturelementet
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Iterera genom varje nod
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Hämta teckensnittsnamn
        Console.WriteLine("Font Name: " + list.Font);

        // Hämta teckensnittslängd
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Hämta teckenstorlek
        Console.WriteLine("Font Size: " + list.FontSize);

        // Hämta teckensnittsfärg
        Console.WriteLine("Font Color: " + list.FontColor);

        // Hämta format
        Console.WriteLine("Font format: " + list.Format);

        // Markera fetstil
        Console.WriteLine("Is bold: " + list.IsBold);

        // Markera kursiv
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### Se även

* class [NumberList](../)
* namnutrymme [Aspose.Note](../../numberlist/)
* hopsättning [Aspose.Note](../../../)


