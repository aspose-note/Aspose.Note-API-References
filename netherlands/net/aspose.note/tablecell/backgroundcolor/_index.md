---
title: TableCell.BackgroundColor
second_title: Aspose.Note voor .NET API-referentie
description: TableCell eigendom. Krijgt of stelt de achtergrondkleur in.
type: docs
weight: 20
url: /nl/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Krijgt of stelt de achtergrondkleur in.

```csharp
public Color BackgroundColor { get; set; }
```

### Voorbeelden

Laat zien hoe u een achtergrondkleur voor een cel instelt.

```csharp
// Maak een object van de klasse Document
Document doc = new Document();

// Initialiseer het klasseobject TableCell en stel tekstinhoud in
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Initialiseer het klasseobject TableRow
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

// Initialiseer het paginaklasse-object
Page page = new Page();
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### Zie ook

* class [TableCell](../)
* naamruimte [Aspose.Note](../../tablecell/)
* montage [Aspose.Note](../../../)


