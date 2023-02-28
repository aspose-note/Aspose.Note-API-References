---
title: Image.VerticalOffset
second_title: Aspose.Note para la referencia de la API de .NET
description: Image propiedad. Obtiene o establece el desplazamiento vertical.
type: docs
weight: 170
url: /es/net/aspose.note/image/verticaloffset/
---
## Image.VerticalOffset property

Obtiene o establece el desplazamiento vertical.

```csharp
public float VerticalOffset { get; set; }
```

### Ejemplos

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

### Ver también

* class [Image](../)
* espacio de nombres [Aspose.Note](../../image/)
* asamblea [Aspose.Note](../../../)


