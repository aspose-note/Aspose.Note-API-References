---
title: TableColumn.LockedWidth
second_title: Aspose.Note for .NET API Reference
description: TableColumn ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν μια στήλη πίνακα έχει κλειδωμένο πλάτος και δεν αλλάζει το μέγεθος αυτόματα ώστε να ταιριάζει στο περιεχόμενο του πίνακα. Από προεπιλογή το πλάτος της στήλης δεν είναι κλειδωμένο.
type: docs
weight: 20
url: /el/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν μια στήλη πίνακα έχει κλειδωμένο πλάτος και δεν αλλάζει το μέγεθος αυτόματα ώστε να ταιριάζει στο περιεχόμενο του πίνακα. Από προεπιλογή, το πλάτος της στήλης δεν είναι κλειδωμένο.

```csharp
public bool LockedWidth { get; set; }
```

### Παραδείγματα

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

### Δείτε επίσης

* class [TableColumn](../)
* χώρος ονομάτων [Aspose.Note](../../tablecolumn/)
* συνέλευση [Aspose.Note](../../../)


