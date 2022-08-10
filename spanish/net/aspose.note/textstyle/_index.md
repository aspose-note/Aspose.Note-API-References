---
title: TextStyle
second_title: Aspose.Note para la referencia de la API de .NET
description: Especifica el estilo de texto.
type: docs
weight: 940
url: /es/net/aspose.note/textstyle/
---
## TextStyle class

Especifica el estilo de texto.

```csharp
public sealed class TextStyle : Style
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TextStyle](textstyle)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default) { get; } | Obtiene el estilo predeterminado para el texto del título en MS OneNote. |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle) { get; } | Obtiene el estilo predeterminado para la fecha del título en MS OneNote. |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle) { get; } | Obtiene el estilo predeterminado para el texto del título en MS OneNote. |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle) { get; } | Obtiene el estilo predeterminado para la hora del título en MS OneNote. |
| [FontColor](../../aspose.note/style/fontcolor) { get; set; } | Obtiene o establece el color de la fuente. |
| [FontName](../../aspose.note/style/fontname) { get; set; } | Obtiene o establece el nombre de la fuente. |
| [FontSize](../../aspose.note/style/fontsize) { get; set; } | Obtiene o establece el tamaño de fuente. |
| [FontStyle](../../aspose.note/style/fontstyle) { get; } | Obtiene el estilo de fuente. |
| [Highlight](../../aspose.note/style/highlight) { get; set; } | Obtiene o establece el color de resaltado. |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress) { get; set; } | Obtiene o establece la dirección del hipervínculo. Debe establecerse si el valor de la[`IsHyperlink`](./ishyperlink) la propiedad es verdadera. |
| [IsBold](../../aspose.note/style/isbold) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto está en negrita. |
| [IsHidden](../../aspose.note/textstyle/ishidden) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto está oculto. |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto es hipervínculo. |
| [IsItalic](../../aspose.note/style/isitalic) { get; set; } | Obtiene o establece un valor que indica si el estilo del texto es cursiva. |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto tiene formato matemático. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto es tachado. |
| [IsSubscript](../../aspose.note/style/issubscript) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto es subíndice. |
| [IsSuperscript](../../aspose.note/style/issuperscript) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto es superíndice. |
| [IsUnderline](../../aspose.note/style/isunderline) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto es subrayado. |
| [Language](../../aspose.note/textstyle/language) { get; set; } | Obtiene o establece el idioma del texto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals#equals_1)(object) | Determina si el objeto especificado es igual al objeto actual. |
| [Equals](../../aspose.note/textstyle/equals#equals)(TextStyle) | Determina si el objeto especificado es igual al objeto actual. |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode)() | Sirve como función hash para el tipo. |

### Ejemplos

Destaquemos los títulos de las páginas entre otros encabezados aumentando el tamaño de la fuente.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Cargue el documento en Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Iterar a través de los títulos de la página.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

Resaltemos los últimos cambios del texto resaltando.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Cargue el documento en Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// Obtenga los nodos RichText modificados la semana pasada.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // Establecer color de resaltado
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // Establecer color de resaltado
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

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

Manipular por formato de texto usando estilo de párrafo.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

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

* class [Style](../style)
* espacio de nombres [Aspose.Note](../../aspose.note)
* asamblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
