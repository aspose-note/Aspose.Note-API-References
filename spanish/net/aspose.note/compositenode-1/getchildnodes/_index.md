---
title: CompositeNode1.GetChildNodes
second_title: Aspose.Note para la referencia de la API de .NET
description: CompositeNode método. Obtener todos los nodos secundarios por tipo de nodo.
type: docs
weight: 70
url: /es/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

Obtener todos los nodos secundarios por tipo de nodo.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parámetro | Descripción |
| --- | --- |
| T1 | El tipo de elementos en la lista devuelta. |

### Valor_devuelto

Una lista de nodos secundarios.

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

Muestra cómo obtener la metainformación de la imagen.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Obtener todos los nodos de imagen
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

### Ver también

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* espacio de nombres [Aspose.Note](../../compositenode-1/)
* asamblea [Aspose.Note](../../../)


