---
title: TableCell.BackgroundColor
second_title: Справочник по API Aspose.Note для .NET
description: TableCell свойство. Получает или задает цвет фона.
type: docs
weight: 20
url: /ru/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

Получает или задает цвет фона.

```csharp
public Color BackgroundColor { get; set; }
```

### Примеры

Показывает, как установить цвет фона для ячейки.

```csharp
// Создаем объект класса Document
Document doc = new Document();

// Инициализируем объект класса TableCell и устанавливаем текстовое содержимое
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Инициализировать объект класса TableRow
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

// Инициализировать объект класса Page
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

### Смотрите также

* class [TableCell](../)
* пространство имен [Aspose.Note](../../tablecell/)
* сборка [Aspose.Note](../../../)


