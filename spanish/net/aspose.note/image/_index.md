---
title: Class Image
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Image clase. Representa una Imagen.
type: docs
weight: 250
url: /es/net/aspose.note/image/
---
## Image class

Representa una Imagen.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Image](image/#constructor)() | Inicializa una nueva instancia del`Image` clase. |
| [Image](image/#constructor_4)(string, Stream) | Inicializa una nueva instancia del`Image` clase. |
| [Image](image/#constructor_5)(string, string, string) | Inicializa una nueva instancia del`Image` clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | Obtiene o establece la alineación. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | Obtiene o establece un cuerpo de texto alternativo para la imagen. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | Obtiene o establece un título de texto alternativo para la imagen. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | Obtiene el almacén de datos de imágenes. |
| [Document](../../aspose.note/node/document/) { get; } | Obtiene el documento del nodo. |
| [FileName](../../aspose.note/image/filename/) { get; } | Obtiene el nombre del archivo. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | Obtiene la ruta al archivo de imagen. |
| [Format](../../aspose.note/image/format/) { get; } | Obtiene el formato de la imagen. |
| [Height](../../aspose.note/image/height/) { get; set; } | Obtiene o establece la altura. Esta es la altura real de la imagen en el documento de MS OneNote. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | Obtiene o establece el desplazamiento horizontal. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | Obtiene o establece el hipervínculo asociado a la imagen. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | Obtiene si la imagen es una imagen de fondo. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Obtiene un valor que indica si este nodo es compuesto. Si es verdadero, el nodo puede tener nodos secundarios. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | Obtiene o establece la hora de la última modificación. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Obtiene el siguiente nodo en el mismo nivel de árbol de nodos. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Obtiene el tipo de nodo. |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | Obtiene la altura original. Este es el ancho original de la imagen, antes de cambiar el tamaño. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | Obtiene el ancho original. Este es el ancho original de la imagen, antes de cambiar el tamaño. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Obtiene el nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Obtiene el nodo anterior en el mismo nivel de árbol de nodos. |
| [Tags](../../aspose.note/image/tags/) { get; } | Obtiene la lista de todas las etiquetas de un párrafo. |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | Obtiene o establece el desplazamiento vertical. |
| [Width](../../aspose.note/image/width/) { get; set; } | Obtiene o establece el ancho. Este es el ancho real de la imagen en el documento de MS OneNote. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | Acepta al visitante del nodo. |

### Ejemplos

Muestra cómo vincular un hipervínculo a una imagen.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://imagen.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Muestra cómo configurar la descripción del texto para una imagen.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

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

Muestra cómo agregar una nueva imagen con etiqueta.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tags();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase Esquema
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Cargar una imagen
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Insertar imagen en el nodo del documento
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Agregar nodo de elemento de contorno
outline.AppendChildLast(outlineElem);

// Agregar nodo de contorno
page.AppendChildLast(outline);

// Añadir nodo de página
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

Muestra cómo agregar una imagen desde un archivo a un documento con propiedades definidas por el usuario.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Cargar documento desde la secuencia.
Document doc = new Document(dataDir + "Aspose.one");

// Obtener la primera página del documento.
Aspose.Note.Page page = doc.FirstChild;

// Carga una imagen del archivo.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Cambia el tamaño de la imagen según tus necesidades (opcional).
                              Width = 100,
                              Height = 100,

                              // Establecer la ubicación de la imagen en la página (opcional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Establecer la alineación de la imagen
                              Alignment = HorizontalAlignment.Right
                          };

// Agrega la imagen a la página.
page.AppendChildLast(image);
```

Muestra cómo agregar una imagen de una secuencia a un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Cargue la segunda imagen usando el nombre de la imagen, la extensión y la transmisión.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Establecer la alineación de la imagen
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Muestra cómo agregar una imagen de un archivo a un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Images();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase Esquema y establece las propiedades de compensación
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Carga una imagen por la ruta del archivo.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Establecer la alineación de la imagen
                              Alignment = HorizontalAlignment.Right
                          };

// Añadir imagen
outlineElem.AppendChildLast(image);

// Agregar elementos de contorno
outline.AppendChildLast(outlineElem);

// Añadir nodo Esquema
page.AppendChildLast(outline);

// Agregar nodo de página
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Ver también

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


