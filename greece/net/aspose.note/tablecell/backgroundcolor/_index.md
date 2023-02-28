---
title: TableCell.BackgroundColor
second_title: Aspose.Note for .NET API Reference
description: TableCell ιδιοκτησία. Παίρνει ή ορίζει το χρώμα φόντου.
type: docs
weight: 20
url: /el/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Παίρνει ή ορίζει το χρώμα φόντου.

```csharp
public Color BackgroundColor { get; set; }
```

### Παραδείγματα

Δείχνει πώς να ορίσετε ένα χρώμα φόντου για ένα κελί.

```csharp
// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης TableCell και ορισμός περιεχομένου κειμένου
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Αρχικοποίηση αντικειμένου κλάσης TableRow
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

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### Δείτε επίσης

* class [TableCell](../)
* χώρος ονομάτων [Aspose.Note](../../tablecell/)
* συνέλευση [Aspose.Note](../../../)


