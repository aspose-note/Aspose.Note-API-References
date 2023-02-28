---
title: TableCell.BackgroundColor
second_title: Aspose.Note per .NET API Reference
description: TableCell proprietà. Ottiene o imposta il colore di sfondo.
type: docs
weight: 20
url: /it/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Ottiene o imposta il colore di sfondo.

```csharp
public Color BackgroundColor { get; set; }
```

### Esempi

Mostra come impostare un colore di sfondo per una cella.

```csharp
// Crea un oggetto della classe Document
Document doc = new Document();

// Inizializza l'oggetto della classe TableCell e imposta il contenuto del testo
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Inizializza l'oggetto della classe TableRow
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

// Inizializza l'oggetto della classe Page
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### Guarda anche

* class [TableCell](../)
* spazio dei nomi [Aspose.Note](../../tablecell/)
* assemblea [Aspose.Note](../../../)


