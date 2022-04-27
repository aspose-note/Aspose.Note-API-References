---
title: TableRow
second_title: Aspose.Note for .NET API Reference
description: 
type: docs
weight: 860
url: /net/aspose.note/tablerow/
---
## TableRow class

Represents a table row.

```csharp
public sealed class TableRow : CompositeNode<TableCell>
```

## Constructors

| Name | Description |
| --- | --- |
| [TableRow](tablerow)() | Initializes a new instance of the [`TableRow`](../tablerow) class. |

## Properties

| Name | Description |
| --- | --- |
| [LastModifiedTime](lastmodifiedtime) { get; set; } | Gets or sets the last modified time. |

## Methods

| Name | Description |
| --- | --- |
| override [Accept](accept)(DocumentVisitor) | Accepts the visitor of the node. |

### Examples

Shows how to get text from every table's row.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tables();

// Load the document into Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Get a list of table nodes
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Iterate through table rows
    foreach (TableRow row in table)
    {
        // Retrieve text
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Print text on the output screen
        Console.WriteLine(text);
    }
}
```

Shows how to get text from a table's cells.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Tables();

// Load the document into Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Get a list of table nodes
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Iterate through table rows
    foreach (TableRow row in table)
    {
        // Get list of TableCell nodes
        // Iterate through table cells
        foreach (TableCell cell in row)
        {
            // Retrieve text
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Print text on the output screen
            Console.WriteLine(text);
        }
    }
}
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [TableCell](../tablecell)
* namespace [Aspose.Note](../../aspose.note)
* assembly [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
