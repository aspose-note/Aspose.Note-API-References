---
title: TableCell.BackgroundColor
second_title: Aspose.Note para la referencia de la API de .NET
description: TableCell propiedad. Obtiene o establece el color de fondo.
type: docs
weight: 20
url: /es/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Obtiene o establece el color de fondo.

```csharp
public Color BackgroundColor { get; set; }
```

### Ejemplos

Muestra cómo establecer un color de fondo para una celda.

```csharp
// Crear un objeto de la clase Documento
Document doc = new Document();

// Inicializa el objeto de la clase TableCell y establece el contenido del texto
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Inicializa el objeto de la clase TableRow
TableRow row = new TableRow();
row.AppendChildLast(cell11);

Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn() { Width = 200 } }
              };
table.AppendChildLast(row);

OutlineElement oe = new OutlineElement();
oe.AppendChildLast(table);

Outline o = new Outline();
o.AppendChildLast(oe);

// Inicializar objeto de clase de página
Page page = new Page();
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### Ver también

* class [TableCell](../)
* espacio de nombres [Aspose.Note](../../tablecell/)
* asamblea [Aspose.Note](../../../)


