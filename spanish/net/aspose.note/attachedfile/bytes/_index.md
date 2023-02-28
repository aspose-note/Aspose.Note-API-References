---
title: AttachedFile.Bytes
second_title: Aspose.Note para la referencia de la API de .NET
description: AttachedFile propiedad. Obtiene los datos binarios de un archivo incrustado.
type: docs
weight: 50
url: /es/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Obtiene los datos binarios de un archivo incrustado.

```csharp
public byte[] Bytes { get; }
```

### Ejemplos

Muestra cómo obtener el contenido de un archivo adjunto.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Attachments();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Obtener una lista de nodos de archivos adjuntos
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Iterar a través de todos los nodos
foreach (AttachedFile file in nodes)
{
    // Cargar archivo adjunto a un objeto de flujo
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Crear un archivo local
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Copiar secuencia de archivos
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### Ver también

* class [AttachedFile](../)
* espacio de nombres [Aspose.Note](../../attachedfile/)
* asamblea [Aspose.Note](../../../)


