---
title: TableColumn.LockedWidth
second_title: Aspose.Note para la referencia de la API de .NET
description: TableColumn propiedad. Obtiene o establece un valor que indica si una columna de la tabla tiene un ancho bloqueado y no cambia de tamaño automáticamente para ajustarse al contenido de la tabla. De manera predeterminada el ancho de la columna no está bloqueado.
type: docs
weight: 20
url: /es/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

Obtiene o establece un valor que indica si una columna de la tabla tiene un ancho bloqueado y no cambia de tamaño automáticamente para ajustarse al contenido de la tabla. De manera predeterminada, el ancho de la columna no está bloqueado.

```csharp
public bool LockedWidth { get; set; }
```

### Ejemplos

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

// Agregar filas
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Agregar nodo de tabla
outlineElem.AppendChildLast(table);

// Agregar nodo de elemento de contorno
outline.AppendChildLast(outlineElem);

// Agregar nodo de contorno
page.AppendChildLast(outline);

// Añadir nodo de página
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

### Ver también

* class [TableColumn](../)
* espacio de nombres [Aspose.Note](../../tablecolumn/)
* asamblea [Aspose.Note](../../../)


