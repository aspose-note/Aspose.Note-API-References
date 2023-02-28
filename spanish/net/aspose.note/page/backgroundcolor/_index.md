---
title: Page.BackgroundColor
second_title: Aspose.Note para la referencia de la API de .NET
description: Page propiedad. Obtiene o establece el color de fondo de la página.
type: docs
weight: 30
url: /es/net/aspose.note/page/backgroundcolor/
---
## Page.BackgroundColor property

Obtiene o establece el color de fondo de la página.

```csharp
public Color BackgroundColor { get; set; }
```

### Ejemplos

Muestra cómo configurar el color de fondo de la página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento de OneNote y obtenga el primer hijo           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
```

Muestra cómo aplicar el estilo de tema oscuro a un documento.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Text();

// Cargue el documento en Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### Ver también

* class [Page](../)
* espacio de nombres [Aspose.Note](../../page/)
* asamblea [Aspose.Note](../../../)


