---
title: TextStyle.IsHyperlink
second_title: Aspose.Note para la referencia de la API de .NET
description: TextStyle propiedad. Obtiene o establece un valor que indica si el estilo de texto es hipervínculo.
type: docs
weight: 80
url: /es/net/aspose.note/textstyle/ishyperlink/
---
## TextStyle.IsHyperlink property

Obtiene o establece un valor que indica si el estilo de texto es hipervínculo.

```csharp
public bool IsHyperlink { get; set; }
```

### Ejemplos

Muestra cómo vincular un hipervínculo a un texto.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tasks();

// Crear un objeto de la clase Documento
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// Agregar elementos de contorno
outline.AppendChildLast(outlineElem);

// Inicializa el objeto de la clase Título
Title title = new Title() { TitleText = titleText };

// Inicializar objeto de clase de página
Page page = new Note.Page() { Title = title };

// Añadir nodo Esquema
page.AppendChildLast(outline);

// Agregar nodo de página
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### Ver también

* class [TextStyle](../)
* espacio de nombres [Aspose.Note](../../textstyle/)
* asamblea [Aspose.Note](../../../)


