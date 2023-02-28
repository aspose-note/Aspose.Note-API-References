---
title: TableCell.BackgroundColor
second_title: Aspose.Note für .NET-API-Referenz
description: TableCell eigendom. Ruft die Hintergrundfarbe ab oder legt sie fest.
type: docs
weight: 20
url: /de/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Ruft die Hintergrundfarbe ab oder legt sie fest.

```csharp
public Color BackgroundColor { get; set; }
```

### Beispiele

Zeigt, wie eine Hintergrundfarbe für eine Zelle festgelegt wird.

```csharp
// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Objekt der TableCell-Klasse initialisieren und Textinhalt festlegen
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// TableRow-Klassenobjekt initialisieren
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

// Seitenklassenobjekt initialisieren
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### Siehe auch

* class [TableCell](../)
* namensraum [Aspose.Note](../../tablecell/)
* Montage [Aspose.Note](../../../)


