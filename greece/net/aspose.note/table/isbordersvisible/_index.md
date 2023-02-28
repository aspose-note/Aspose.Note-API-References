---
title: Table.IsBordersVisible
second_title: Aspose.Note for .NET API Reference
description: Table ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το περίγραμμα του πίνακα είναι ορατό.
type: docs
weight: 30
url: /el/net/aspose.note/table/isbordersvisible/
---
## Table.IsBordersVisible property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το περίγραμμα του πίνακα είναι ορατό.

```csharp
public bool IsBordersVisible { get; set; }
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

Δείχνει πώς να προσθέσετε νέο πίνακα με ετικέτα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης TableRow
TableRow row = new TableRow(doc);

// Αρχικοποίηση αντικειμένου κλάσης TableCell
TableCell cell = new TableCell(doc);

// Εισαγωγή περιεχομένου κελιού
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Προσθήκη κελιού στον κόμβο γραμμής
row.AppendChildLast(cell);

// Αρχικοποίηση κόμβου πίνακα
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Εισαγωγή κόμβου γραμμής στον πίνακα
table.AppendChildLast(row);

// Προσθήκη ετικέτας σε αυτόν τον κόμβο πίνακα
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Προσθήκη κόμβου πίνακα
outlineElem.AppendChildLast(table);

// Προσθήκη στοιχείων περιγράμματος
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Δείχνει πώς να δημιουργήσετε έναν πίνακα με κλειδωμένη στήλη.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tables();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης TableRow
TableRow row1 = new TableRow(doc);

// Αρχικοποίηση αντικειμένου κλάσης TableCell και ορισμός περιεχομένου κειμένου
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Αρχικοποίηση αντικειμένου κλάσης TableRow
TableRow row2 = new TableRow(doc);

// Αρχικοποίηση αντικειμένου κλάσης TableCell και ορισμός περιεχομένου κειμένου
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Αρχικοποίηση αντικειμένου κλάσης πίνακα
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Προσθήκη σειρών
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// Προσθήκη κόμβου πίνακα
outlineElem.AppendChildLast(table);

// Προσθήκη κόμβου στοιχείου περιγράμματος
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου περιγράμματος
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Δείχνει πώς να δημιουργήσετε έναν νέο πίνακα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tables();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης TableRow
TableRow row1 = new TableRow(doc);

// Εκκίνηση αντικειμένων κλάσης TableCell
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Προσθήκη στοιχείων περιγράμματος στο κελί του πίνακα
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Πίνακας κελιών σε σειρές
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Αρχικοποίηση αντικειμένου κλάσης TableRow
TableRow row2 = new TableRow(doc);

// αρχικοποίηση αντικειμένων κλάσης TableCell
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Προσθήκη στοιχείων περιγράμματος στο κελί του πίνακα
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Προσθήκη κελιών πίνακα σε γραμμές
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Αρχικοποίηση αντικειμένου κλάσης πίνακα και ορισμός πλάτη στηλών
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Προσθήκη σειρών πίνακα στον πίνακα
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Αρχικοποίηση αντικειμένου Outline
Outline outline = new Outline(doc);

// Αρχικοποίηση αντικειμένου OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Προσθήκη πίνακα στον κόμβο στοιχείου περιγράμματος
outlineElem.AppendChildLast(table);

// Προσθήκη στοιχείου περιγράμματος στο περίγραμμα
outline.AppendChildLast(outlineElem);

// Προσθήκη περίγραμμα στον κόμβο σελίδας
page.AppendChildLast(outline);

// Προσθήκη σελίδας στον κόμβο εγγράφου
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Δείτε επίσης

* class [Table](../)
* χώρος ονομάτων [Aspose.Note](../../table/)
* συνέλευση [Aspose.Note](../../../)


