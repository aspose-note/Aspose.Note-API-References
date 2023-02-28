---
title: Image.Tags
second_title: Aspose.Note para la referencia de la API de .NET
description: Image propiedad. Obtiene la lista de todas las etiquetas de un párrafo.
type: docs
weight: 160
url: /es/net/aspose.note/image/tags/
---
## Image.Tags property

Obtiene la lista de todas las etiquetas de un párrafo.

```csharp
public List<ITag> Tags { get; }
```

### Ejemplos

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

### Ver también

* interface [ITag](../../itag/)
* class [Image](../)
* espacio de nombres [Aspose.Note](../../image/)
* asamblea [Aspose.Note](../../../)


