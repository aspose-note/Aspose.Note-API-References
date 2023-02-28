---
title: Notebook.DisplayName
second_title: Aspose.Note para la referencia de la API de .NET
description: Notebook propiedad. Obtiene o establece el nombre para mostrar.
type: docs
weight: 40
url: /es/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

Obtiene o establece el nombre para mostrar.

```csharp
public string DisplayName { get; set; }
```

### Ejemplos

Muestra cómo eliminar una sección de un bloc de notas.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Cargar un cuaderno de OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Atraviesa sus nodos secundarios para buscar el elemento secundario deseado
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Eliminar el elemento secundario del cuaderno
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Guardar el cuaderno
notebook.Save(dataDir);
```

### Ver también

* class [Notebook](../)
* espacio de nombres [Aspose.Note](../../notebook/)
* asamblea [Aspose.Note](../../../)


