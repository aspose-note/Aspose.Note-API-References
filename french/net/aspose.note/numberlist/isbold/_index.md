---
title: NumberList.IsBold
second_title: Référence de l'API Aspose.Note pour .NET
description: NumberList propriété. Obtient ou définit une valeur indiquant si le style de texte est en gras.
type: docs
weight: 60
url: /fr/net/aspose.note/numberlist/isbold/
---
## NumberList.IsBold property

Obtient ou définit une valeur indiquant si le style de texte est en gras.

```csharp
public bool IsBold { get; set; }
```

### Exemples

Montre comment récupérer des informations sur le formatage de la liste.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Charge le document dans Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Récupère une collection de nœuds de l'élément de contour
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Itérer à travers chaque nœud
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Récupérer le nom de la police
        Console.WriteLine("Font Name: " + list.Font);

        // Récupère la longueur de la police
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Récupère la taille de la police
        Console.WriteLine("Font Size: " + list.FontSize);

        // Récupère la couleur de la police
        Console.WriteLine("Font Color: " + list.FontColor);

        // Récupérer le format
        Console.WriteLine("Font format: " + list.Format);

        // Cochez gras
        Console.WriteLine("Is bold: " + list.IsBold);

        // Vérifier l'italique
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### Voir également

* class [NumberList](../)
* espace de noms [Aspose.Note](../../numberlist/)
* Assemblée [Aspose.Note](../../../)


