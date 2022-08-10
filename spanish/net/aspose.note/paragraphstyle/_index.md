---
title: ParagraphStyle
second_title: Aspose.Note para la referencia de la API de .NET
description: Configuración de estilo de texto que se usará si no hay un objeto TextStyle coincidente enStyles colección este objeto no especifica una configuración necesaria.
type: docs
weight: 490
url: /es/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

Configuración de estilo de texto que se usará si no hay un objeto TextStyle coincidente enStyles colección este objeto no especifica una configuración necesaria.

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ParagraphStyle](paragraphstyle)() | Inicializa una nueva instancia del[`ParagraphStyle`](../paragraphstyle) clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default) { get; } | Obtiene ParagraphStyle con la configuración predeterminada. |
| [FontColor](../../aspose.note/style/fontcolor) { get; set; } | Obtiene o establece el color de la fuente. |
| [FontName](../../aspose.note/style/fontname) { get; set; } | Obtiene o establece el nombre de la fuente. |
| [FontSize](../../aspose.note/style/fontsize) { get; set; } | Obtiene o establece el tamaño de fuente. |
| [FontStyle](../../aspose.note/style/fontstyle) { get; } | Obtiene el estilo de fuente. |
| [Highlight](../../aspose.note/style/highlight) { get; set; } | Obtiene o establece el color de resaltado. |
| [IsBold](../../aspose.note/style/isbold) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto está en negrita. |
| [IsItalic](../../aspose.note/style/isitalic) { get; set; } | Obtiene o establece un valor que indica si el estilo del texto es cursiva. |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto es tachado. |
| [IsSubscript](../../aspose.note/style/issubscript) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto es subíndice. |
| [IsSuperscript](../../aspose.note/style/issuperscript) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto es superíndice. |
| [IsUnderline](../../aspose.note/style/isunderline) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto es subrayado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals#equals_1)(object) | Determina si el objeto especificado es igual al objeto actual. |
| [Equals](../../aspose.note/paragraphstyle/equals#equals)(ParagraphStyle) | Determina si el objeto especificado es igual al objeto actual. |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode)() | Sirve como función hash para el tipo. |

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

Muestra cómo insertar una nueva lista con numeración china.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Inicializa el documento de OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// Inicializar la página de OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Aplicar la configuración de estilo de texto
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Los números en el mismo esquema se incrementan automáticamente.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Muestra cómo insertar nuevas listas con viñetas.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crear un objeto de la clase Documento
Aspose.Note.Document doc = new Aspose.Note.Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase Esquema
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase TextStyle y establece las propiedades de formato
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inicializar objetos de la clase OutlineElement y aplicar viñetas
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// Inicializa el objeto de la clase RichText y aplica el estilo de texto
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Agregar elementos de contorno
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Añadir nodo Esquema
page.AppendChildLast(outline);
// Agregar nodo de página
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

Muestra cómo insertar una nueva lista con numeración.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase Esquema
Outline outline = new Outline(doc);

// Inicializa el objeto de la clase TextStyle y establece las propiedades de formato
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Inicializar los objetos de la clase OutlineElement y aplicar la numeración
// Los números en el mismo esquema se incrementan automáticamente.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Agregar elementos de contorno
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Añadir nodo Esquema
page.AppendChildLast(outline);

// Agregar nodo de página
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Ver también

* class [Style](../style)
* espacio de nombres [Aspose.Note](../../aspose.note)
* asamblea [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
