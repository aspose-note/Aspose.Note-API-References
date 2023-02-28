---
title: Image.HyperlinkUrl
second_title: Aspose.Note para la referencia de la API de .NET
description: Image propiedad. Obtiene o establece el hipervínculo asociado a la imagen.
type: docs
weight: 110
url: /es/net/aspose.note/image/hyperlinkurl/
---
## Image.HyperlinkUrl property

Obtiene o establece el hipervínculo asociado a la imagen.

```csharp
public string HyperlinkUrl { get; set; }
```

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

### Ver también

* class [Image](../)
* espacio de nombres [Aspose.Note](../../image/)
* asamblea [Aspose.Note](../../../)


