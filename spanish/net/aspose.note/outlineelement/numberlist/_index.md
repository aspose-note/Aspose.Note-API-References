---
title: NumberList
second_title: Aspose.Note para la referencia de la API de .NET
description: Obtiene o establece el estilo del encabezado de la lista numerada.
type: docs
weight: 50
url: /es/net/aspose.note/outlineelement/numberlist/
---
## OutlineElement.NumberList property

Obtiene o establece el estilo del encabezado de la lista numerada.

```csharp
public NumberList NumberList { get; set; }
```

### Ejemplos

Muestra cómo recuperar información sobre el formato de la lista.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Recuperar una colección de nodos del elemento de esquema
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

* class [NumberList](../../numberlist)
* class [OutlineElement](../../outlineelement)
* espacio de nombres [Aspose.Note](../../outlineelement)
* asamblea [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
