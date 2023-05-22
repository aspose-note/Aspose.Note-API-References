---
title: Table.Columns
second_title: Aspose.Note for .NET API Reference
description: Table property. Gets the columns of the table
type: docs
weight: 20
url: /net/aspose.note/table/columns/
---
## Table.Columns property

Gets the columns of the table.

```csharp
public IList<TableColumn> Columns { get; }
```

## Examples

Shows how to set a background color for a cell.

```csharp
// Create an object of the Document class
Document doc = new Document();

// Initialize TableCell class object and set text content
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Initialize TableRow class object
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

// Initialize Page class object
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

Shows how to add new table with tag.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tags();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize TableRow class object
TableRow row = new TableRow(doc);

// Initialize TableCell class object
TableCell cell = new TableCell(doc);

// Insert cell content
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Add cell to row node
row.AppendChildLast(cell);

// Initialize table node
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Insert row node in table
table.AppendChildLast(row);

// Add tag to this table node
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Add table node
outlineElem.AppendChildLast(table);

// Add outline elements
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Save OneNote document
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Shows how to create a table with a locked column.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tables();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize TableRow class object
TableRow row1 = new TableRow(doc);

// Initialize TableCell class object and set text content
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Initialize TableRow class object
TableRow row2 = new TableRow(doc);

// Initialize TableCell class object and set text content
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Initialize Table class object
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Add rows
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Add table node
outlineElem.AppendChildLast(table);

// Add outline element node
outline.AppendChildLast(outlineElem);

// Add outline node
page.AppendChildLast(outline);

// Add page node
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Shows how to create a new table.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tables();

// Create an object of the Document class
Document doc = new Document();

// Initialize Page class object
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Initialize TableRow class object
TableRow row1 = new TableRow(doc);

// Initialize TableCell class objects
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Append outline elements in the table cell
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Table cells to rows
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Initialize TableRow class object
TableRow row2 = new TableRow(doc);

// initialize TableCell class objects
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Append outline elements in the table cell
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Append table cells to rows
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Initialize Table class object and set column widths
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Append table rows to table
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Initialize Outline object
Outline outline = new Outline(doc);

// Initialize OutlineElement object
OutlineElement outlineElem = new OutlineElement(doc);

// Add table to outline element node
outlineElem.AppendChildLast(table);

// Add outline element to outline
outline.AppendChildLast(outlineElem);

// Add outline to page node
page.AppendChildLast(outline);

// Add page to document node
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### See Also

* class [TableColumn](../../tablecolumn/)
* class [Table](../)
* namespace [Aspose.Note](../../table/)
* assembly [Aspose.Note](../../../)


