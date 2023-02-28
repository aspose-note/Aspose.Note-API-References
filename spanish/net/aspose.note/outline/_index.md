---
title: Class Outline
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Outline clase. Representa un esquema.
type: docs
weight: 450
url: /es/net/aspose.note/outline/
---
## Outline class

Representa un esquema.

```csharp
public sealed class Outline : IndentatedNode<IOutlineChildNode>, IPageChildNode
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Outline](outline/#constructor)() | Inicializa una nueva instancia del`Outline` clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DescendantsCannotBeMoved](../../aspose.note/outline/descendantscannotbemoved/) { get; set; } | Obtiene si los descendientes del contorno se pueden mover. |
| [Document](../../aspose.note/node/document/) { get; } | Obtiene el documento del nodo. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [HorizontalOffset](../../aspose.note/outline/horizontaloffset/) { get; set; } | Obtiene o establece el desplazamiento horizontal. |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/outline/lastmodifiedtime/) { get; set; } | Obtiene o establece la hora de última modificación. |
| [MaxHeight](../../aspose.note/outline/maxheight/) { get; set; } | Obtiene o establece la altura máxima. |
| [MaxWidth](../../aspose.note/outline/maxwidth/) { get; set; } | Obtiene o establece el ancho máximo. |
| [MinWidth](../../aspose.note/outline/minwidth/) { get; set; } | Obtiene o establece el ancho mínimo. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Obtiene el siguiente nodo en el mismo nivel de árbol de nodos. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Obtiene el tipo de nodo. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Obtiene el nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Obtiene el nodo anterior en el mismo nivel de árbol de nodos. |
| [ReservedWidth](../../aspose.note/outline/reservedwidth/) { get; set; } | Obtiene o establece el ancho reservado. |
| [VerticalOffset](../../aspose.note/outline/verticaloffset/) { get; set; } | Obtiene o establece el desplazamiento vertical. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Accept](../../aspose.note/outline/accept/)(DocumentVisitor) | Acepta al visitante del nodo. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

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

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


