---
title: RichText.Tags
second_title: Aspose.Note para la referencia de la API de .NET
description: RichText propiedad. Obtiene la lista de todas las etiquetas de un párrafo.
type: docs
weight: 90
url: /es/net/aspose.note/richtext/tags/
---
## RichText.Tags property

Obtiene la lista de todas las etiquetas de un párrafo.

```csharp
public List<ITag> Tags { get; }
```

### Ejemplos

Muestra cómo acceder a los detalles de las tareas de Outlook.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tasks();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Obtener todos los nodos RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// Iterar a través de cada nodo
foreach (RichText richText in nodes)
{
    var tasks = richText.Tags.OfType<NoteTask>();
    if (tasks.Any())
    {
        Console.WriteLine($"Task: {richText.Text}");
        foreach (var noteTask in tasks)
        {
            // Recuperar propiedades
            Console.WriteLine($"    Completed Time: {noteTask.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTask.CreationTime}");
            Console.WriteLine($"    Due Date: {noteTask.DueDate}");
            Console.WriteLine($"    Status: {noteTask.Status}");
            Console.WriteLine($"    Icon: {noteTask.Icon}");
        }
    }
}
```

### Ver también

* interface [ITag](../../itag/)
* class [RichText](../)
* espacio de nombres [Aspose.Note](../../richtext/)
* asamblea [Aspose.Note](../../../)


