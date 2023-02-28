---
title: CheckBox.SetOpen
second_title: Aspose.Note para la referencia de la API de .NET
description: CheckBox método. Establece la etiqueta en estado abierto.
type: docs
weight: 80
url: /es/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

Establece la etiqueta en estado abierto.

```csharp
public virtual void SetOpen()
```

### Ejemplos

Muestra cómo abrir todas las casillas de verificación relacionadas con el 'Proyecto C'.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tags();

// Cargue el documento en Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

### Ver también

* class [CheckBox](../)
* espacio de nombres [Aspose.Note](../../checkbox/)
* asamblea [Aspose.Note](../../../)


