---
title: NumberList.Font
second_title: Aspose.Note para la referencia de la API de .NET
description: NumberList propiedad. Obtiene o establece el nombre de la fuente.
type: docs
weight: 20
url: /es/net/aspose.note/numberlist/font/
---
## NumberList.Font property

Obtiene o establece el nombre de la fuente.

```csharp
public string Font { get; set; }
```

### Ejemplos

Muestra cómo recuperar información sobre el formato de la lista.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Recuperar una colección de nodos del elemento de contorno
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Iterar a través de cada nodo
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Recuperar el nombre de la fuente
        Console.WriteLine("Font Name: " + list.Font);

        // Recuperar la longitud de la fuente
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Recuperar tamaño de letra
        Console.WriteLine("Font Size: " + list.FontSize);

        // Recuperar el color de la fuente
        Console.WriteLine("Font Color: " + list.FontColor);

        // Recuperar formato
        Console.WriteLine("Font format: " + list.Format);

        // Marque en negrita
        Console.WriteLine("Is bold: " + list.IsBold);

        // Comprobar cursiva
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### Ver también

* class [NumberList](../)
* espacio de nombres [Aspose.Note](../../numberlist/)
* asamblea [Aspose.Note](../../../)


