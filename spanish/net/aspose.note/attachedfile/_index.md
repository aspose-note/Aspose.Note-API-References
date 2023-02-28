---
title: Class AttachedFile
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.AttachedFile clase. Representa un archivo adjunto.
type: docs
weight: 10
url: /es/net/aspose.note/attachedfile/
---
## AttachedFile class

Representa un archivo adjunto.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AttachedFile](attachedfile/#constructor)() | Inicializa una nueva instancia del`AttachedFile` clase. |
| [AttachedFile](attachedfile/#constructor_6)(string, Stream) | Inicializa una nueva instancia del`AttachedFile` clase. |
| [AttachedFile](attachedfile/#constructor_7)(string, Stream, ImageFormat) | Inicializa una nueva instancia del`AttachedFile` clase. |
| [AttachedFile](attachedfile/#constructor_8)(string, Stream, Stream, ImageFormat) | Inicializa una nueva instancia del`AttachedFile` clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment/) { get; set; } | Obtiene o establece la alineación. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription/) { get; set; } | Obtiene o establece un cuerpo de texto alternativo para el icono del archivo adjunto. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle/) { get; set; } | Obtiene o establece un título de texto alternativo para el icono del archivo adjunto. |
| [Bytes](../../aspose.note/attachedfile/bytes/) { get; } | Obtiene los datos binarios de un archivo incrustado. |
| [Document](../../aspose.note/node/document/) { get; } | Obtiene el documento del nodo. |
| [Extension](../../aspose.note/attachedfile/extension/) { get; } | Obtiene la extensión de un archivo incrustado. |
| [FileName](../../aspose.note/attachedfile/filename/) { get; } | Obtiene el nombre del archivo incrustado. |
| [FilePath](../../aspose.note/attachedfile/filepath/) { get; } | Obtiene la ruta al archivo original. |
| [Height](../../aspose.note/attachedfile/height/) { get; } | Obtiene la altura original del icono del archivo incrustado. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset/) { get; set; } | Obtiene o establece el desplazamiento horizontal. |
| [Icon](../../aspose.note/attachedfile/icon/) { get; } | Obtiene los datos binarios del icono asociado con el archivo incrustado. |
| [IconExtension](../../aspose.note/attachedfile/iconextension/) { get; } | Obtiene la extensión del icono. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Obtiene un valor que indica si este nodo es compuesto. Si es verdadero, el nodo puede tener nodos secundarios. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout/) { get; set; } | Obtiene o establece un valor que indica si la vista del archivo es de impresión. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser/) { get; set; } | Obtiene o establece un valor que indica si el usuario actualizó explícitamente el valor del tamaño del icono. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime/) { get; set; } | Obtiene o establece la hora de última modificación. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight/) { get; set; } | Obtiene o establece la altura máxima para mostrar el icono del archivo incrustado. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth/) { get; set; } | Obtiene o establece el ancho máximo para mostrar el icono del archivo incrustado. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Obtiene el siguiente nodo en el mismo nivel de árbol de nodos. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Obtiene el tipo de nodo. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Obtiene el nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Obtiene el nodo anterior en el mismo nivel de árbol de nodos. |
| [Tags](../../aspose.note/attachedfile/tags/) { get; } | Obtiene la lista de todas las etiquetas de un párrafo. |
| [Text](../../aspose.note/attachedfile/text/) { get; set; } | Obtiene o establece la representación de texto del archivo incrustado. La cadena NO DEBE contener ningún carácter del valor 10 (avance de línea) o 13 (retorno de carro). |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset/) { get; set; } | Obtiene o establece el desplazamiento vertical. |
| [Width](../../aspose.note/attachedfile/width/) { get; } | Obtiene el ancho original del icono del archivo incrustado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept/)(DocumentVisitor) | Acepta al visitante del nodo. |

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

Muestra cómo agregar un archivo a un documento mediante la ruta de archivo.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase Esquema
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Inicializa el objeto de la clase AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Agregar archivo adjunto
outlineElem.AppendChildLast(attachedFile);

// Agregar nodo de elemento de contorno
outline.AppendChildLast(outlineElem);

// Agregar nodo de contorno
page.AppendChildLast(outline);

// Añadir nodo de página
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

Muestra cómo agregar un archivo de una secuencia a un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Attachments();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase Esquema
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Inicializa el objeto de clase AttachedFile y también pasa su ruta de icono
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Agregar archivo adjunto
    outlineElem.AppendChildLast(attachedFile);
}

// Agregar nodo de elemento de contorno
outline.AppendChildLast(outlineElem);

// Agregar nodo de contorno
page.AppendChildLast(outline);

// Añadir nodo de página
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

### Ver también

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


