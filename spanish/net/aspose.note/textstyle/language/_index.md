---
title: TextStyle.Language
second_title: Aspose.Note para la referencia de la API de .NET
description: TextStyle propiedad. Obtiene o establece el idioma del texto.
type: docs
weight: 100
url: /es/net/aspose.note/textstyle/language/
---
## TextStyle.Language property

Obtiene o establece el idioma del texto.

```csharp
public CultureInfo Language { get; set; }
```

### Observaciones

DevolucionesInvariantCulture si la propiedad no está establecida.

### Ejemplos

Establecer el idioma de prueba para un texto.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

### Ver también

* class [TextStyle](../)
* espacio de nombres [Aspose.Note](../../textstyle/)
* asamblea [Aspose.Note](../../../)


