---
title: Columns
second_title: Aspose.Note para la referencia de la API de .NET
description: Obtiene las columnas de la tabla.
type: docs
weight: 20
url: /es/net/aspose.note/table/columns/
---
## Table.Columns property

Obtiene las columnas de la tabla.

```csharp
public IList<TableColumn> Columns { get; }
```

### Ejemplos

Muestra cómo establecer un color de fondo para una celda.

```csharp
// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializa el objeto de la clase TableCell y establece el contenido del texto
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Inicializa el objeto de la clase TableRow
TableRow row = new TableRow(doc);
row.AppendChildLast(cell11);

Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn() { Width = 200 } }
              };
table.AppendChildLast(row);

OutlineElement oe = new OutlineElement(doc);
oe.AppendChildLast(table);

Outline o = new Outline(doc);
o.AppendChildLast(oe);

// Inicializar objeto de clase de página
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

Muestra cómo agregar una nueva tabla con etiqueta.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tags();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase TableRow
TableRow row = new TableRow(doc);

// Inicializa el objeto de la clase TableCell
TableCell cell = new TableCell(doc);

// Insertar contenido de celda
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Agregar celda al nodo de fila
row.AppendChildLast(cell);

// Inicializa el nodo de la tabla
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Insertar nodo de fila en la tabla
table.AppendChildLast(row);

// Agregar etiqueta a este nodo de tabla
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Agregar nodo de tabla
outlineElem.AppendChildLast(table);

// Agregar elementos de contorno
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Guardar documento de OneNote
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Muestra cómo crear una tabla con una columna bloqueada.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tables();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase TableRow
TableRow row1 = new TableRow(doc);

// Inicializa el objeto de la clase TableCell y establece el contenido del texto
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Inicializa el objeto de la clase TableRow
TableRow row2 = new TableRow(doc);

// Inicializa el objeto de la clase TableCell y establece el contenido del texto
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Inicializa el objeto de la clase Table
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Añadir filas
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Agregar nodo de tabla
outlineElem.AppendChildLast(table);

// Agregar nodo de elemento de esquema
outline.AppendChildLast(outlineElem);

// Agregar nodo de esquema
page.AppendChildLast(outline);

// Añadir nodo de página
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Muestra cómo crear una nueva tabla.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Tables();

// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializar objeto de clase de página
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Inicializa el objeto de la clase TableRow
TableRow row1 = new TableRow(doc);

// Inicializar objetos de la clase TableCell
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Agregar elementos de contorno en la celda de la tabla
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Tabla de celdas a filas
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Inicializa el objeto de la clase TableRow
TableRow row2 = new TableRow(doc);

// inicializa los objetos de la clase TableCell
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Agregar elementos de contorno en la celda de la tabla
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Agregar celdas de la tabla a las filas
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Inicializa el objeto de la clase Table y establece el ancho de las columnas
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Agregar filas de la tabla a la tabla
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Inicializa el objeto Esquema
Outline outline = new Outline(doc);

// Inicializa el objeto OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Agregar tabla al nodo del elemento de contorno
outlineElem.AppendChildLast(table);

// Agregar elemento de contorno al contorno
outline.AppendChildLast(outlineElem);

// Agregar esquema al nodo de la página
page.AppendChildLast(outline);

// Agregar página al nodo del documento
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Ver también

* class [TableColumn](../../tablecolumn)
* class [Table](../../table)
* espacio de nombres [Aspose.Note](../../table)
* asamblea [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
