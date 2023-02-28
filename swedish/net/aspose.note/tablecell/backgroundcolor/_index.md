---
title: TableCell.BackgroundColor
second_title: Aspose.Note för .NET API-referens
description: TableCell fast egendom. Hämtar eller ställer in bakgrundsfärgen.
type: docs
weight: 20
url: /sv/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Hämtar eller ställer in bakgrundsfärgen.

```csharp
public Color BackgroundColor { get; set; }
```

### Exempel

Visar hur man ställer in en bakgrundsfärg för en cell.

```csharp
// Skapa ett objekt av klassen Document
Document doc = new Document();

// Initiera TableCell-klassobjekt och ställ in textinnehåll
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Initiera TableRow-klassobjekt
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

// Initiera Sidklassobjekt
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### Se även

* class [TableCell](../)
* namnutrymme [Aspose.Note](../../tablecell/)
* hopsättning [Aspose.Note](../../../)


