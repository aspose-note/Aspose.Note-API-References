---
title: Interface INoteTag
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.INoteTag interfaz. La interfaz para etiquetas de notas es decir etiquetas que no están asociadas con tareas de Outlook.
type: docs
weight: 180
url: /es/net/aspose.note/inotetag/
---
## INoteTag interface

La interfaz para etiquetas de notas (es decir, etiquetas que no están asociadas con tareas de Outlook).

```csharp
public interface INoteTag : ITag
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FontColor](../../aspose.note/inotetag/fontcolor/) { get; set; } | Obtiene o establece el color de la fuente. |
| [Highlight](../../aspose.note/inotetag/highlight/) { get; set; } | Obtiene o establece el color de resaltado. |
| [Label](../../aspose.note/inotetag/label/) { get; set; } | Obtiene o establece el texto de la etiqueta. |

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

* interface [ITag](../itag/)
* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


