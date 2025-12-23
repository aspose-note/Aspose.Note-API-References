---
title: TableCell.BackgroundColor
second_title: Aspose.Note for .NET API Reference
description: TableCell property. Gets or sets the background color
type: docs
weight: 20
url: /net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Gets or sets the background color.

```csharp
public Color BackgroundColor { get; set; }
```

## Examples

Shows how to set a background color for a cell.

```csharp
// Create an object of the Document class
Document doc = new Document();

// Initialize TableCell class object and set text content
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText("Small text"));
cell11.BackgroundColor = Color.Coral;

// Initialize TableRow class object
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

// Initialize Page class object
Page page = new Page();
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### See Also

* class [TableCell](../)
* namespace [Aspose.Note](../../tablecell/)
* assembly [Aspose.Note](../../../)


