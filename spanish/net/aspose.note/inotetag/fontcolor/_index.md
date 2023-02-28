---
title: INoteTag.FontColor
second_title: Aspose.Note para la referencia de la API de .NET
description: INoteTag propiedad. Obtiene o establece el color de la fuente.
type: docs
weight: 10
url: /es/net/aspose.note/inotetag/fontcolor/
---
## INoteTag.FontColor property

Obtiene o establece el color de la fuente.

```csharp
public Color FontColor { get; set; }
```

### Ejemplos

Muestra cómo acceder a los detalles de una etiqueta.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tags();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// Obtener todos los nodos RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterar a través de cada nodo
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // Recuperar propiedades
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

### Ver también

* interface [INoteTag](../)
* espacio de nombres [Aspose.Note](../../inotetag/)
* asamblea [Aspose.Note](../../../)


