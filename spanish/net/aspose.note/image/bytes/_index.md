---
title: Image.Bytes
second_title: Aspose.Note para la referencia de la API de .NET
description: Image propiedad. Obtiene el almacén de datos de imágenes.
type: docs
weight: 50
url: /es/net/aspose.note/image/bytes/
---
## Image.Bytes property

Obtiene el almacén de datos de imágenes.

```csharp
public byte[] Bytes { get; }
```

### Ejemplos

Muestra cómo obtener una imagen de un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Obtener todos los nodos de imagen
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Guardar bytes de imagen en un archivo
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### Ver también

* class [Image](../)
* espacio de nombres [Aspose.Note](../../image/)
* asamblea [Aspose.Note](../../../)


