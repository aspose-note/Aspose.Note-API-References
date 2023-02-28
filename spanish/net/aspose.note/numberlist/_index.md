---
title: Class NumberList
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.NumberList clase. Representa la lista numerada o con viñetas.
type: docs
weight: 440
url: /es/net/aspose.note/numberlist/
---
## NumberList class

Representa la lista numerada o con viñetas.

```csharp
public class NumberList
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | Inicializa una nueva instancia del`NumberList`class. Esta instancia representa una lista con viñetas. |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | Inicializa una nueva instancia del`NumberList` class. Esta instancia representa una lista numerada. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | Obtiene o establece el nombre de la fuente. |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | Obtiene o establece el color de la fuente. |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | Obtiene o establece el tamaño de fuente. |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | Obtiene o establece el formato del encabezado de línea. Para listas con viñetas representa un símbolo de viñeta. |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | Obtiene o establece un valor que indica si el estilo de texto está en negrita. |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | Obtiene o establece un valor que indica si el estilo del texto es cursiva. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | Obtiene o establece la hora de última modificación. |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | Obtiene o establece el formato de número utilizado para un grupo de objetos numerados automáticamente. Debería ser nulo para listas con viñetas. |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | Obtiene o establece el valor numérico que anula el valor numérico automático del elemento de la lista. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | Determina si el objeto especificado es igual al objeto actual. |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | Determina si el objeto especificado es igual al objeto actual. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | Sirve como función hash para el tipo. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | Obtiene el encabezado de la lista numerada. |

### Ejemplos

Muestra cómo recuperar información sobre el formato de la lista.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Recuperar una colección de nodos del elemento de contorno
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Iterar a través de cada nodo
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Recuperar el nombre de la fuente
        Console.WriteLine("Font Name: " + list.Font);

        // Recuperar la longitud de la fuente
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Recuperar tamaño de letra
        Console.WriteLine("Font Size: " + list.FontSize);

        // Recuperar el color de la fuente
        Console.WriteLine("Font Color: " + list.FontColor);

        // Recuperar formato
        Console.WriteLine("Font format: " + list.Format);

        // Marque en negrita
        Console.WriteLine("Is bold: " + list.IsBold);

        // Comprobar cursiva
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
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

* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


