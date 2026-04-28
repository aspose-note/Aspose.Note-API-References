---
title: Table.IsBordersVisible
second_title: Справочник по API Aspose.Note для .NET
description: Table свойство. Получает или задает значение указывающее видна ли граница таблицы.
type: docs
weight: 30
url: /ru/net/aspose.note/table/isbordersvisible/
---
## Table.IsBordersVisible property

Получает или задает значение, указывающее, видна ли граница таблицы.

```csharp
public bool IsBordersVisible { get; set; }
```

### Примеры

Показывает, как установить цвет фона для ячейки.

```csharp
// Создаем объект класса Document
Document doc = new Document();

// Инициализируем объект класса TableCell и устанавливаем текстовое содержимое
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// Инициализировать объект класса TableRow
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

// Инициализировать объект класса Page
Page page = new Page();
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

Показывает, как добавить новую таблицу с тегом.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса TableRow
TableRow row = new TableRow();

// Инициализировать объект класса TableCell
TableCell cell = new TableCell();

// Вставляем содержимое ячейки
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Добавляем ячейку в узел строки
row.AppendChildLast(cell);

// Инициализировать узел таблицы
Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Вставляем узел строки в таблицу
table.AppendChildLast(row);

// Добавляем тег к этому узлу таблицы
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline();
OutlineElement outlineElem = new OutlineElement();

// Добавляем узел таблицы
outlineElem.AppendChildLast(table);

// Добавляем элементы контура
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

Показывает, как создать таблицу с заблокированным столбцом.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tables();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса TableRow
TableRow row1 = new TableRow();

// Инициализируем объект класса TableCell и устанавливаем текстовое содержимое
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Инициализировать объект класса TableRow
TableRow row2 = new TableRow();

// Инициализируем объект класса TableCell и устанавливаем текстовое содержимое
TableCell cell21 = new TableCell();
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Инициализировать объект класса Table
Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Добавляем строки
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline();
OutlineElement outlineElem = new OutlineElement();

// Добавляем узел таблицы
outlineElem.AppendChildLast(table);

// Добавляем узел элемента контура
outline.AppendChildLast(outlineElem);

// Добавляем узел контура
page.AppendChildLast(outline);

// Добавляем узел страницы
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

Показывает, как создать новую таблицу.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tables();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса TableRow
TableRow row1 = new TableRow();

// Инициализировать объекты класса TableCell
TableCell cell11 = new TableCell();
TableCell cell12 = new TableCell();
TableCell cell13 = new TableCell();

// Добавляем элементы контура в ячейку таблицы
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Ячейки таблицы в строки
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Инициализировать объект класса TableRow
TableRow row2 = new TableRow();

// инициализируем объекты класса TableCell
TableCell cell21 = new TableCell();
TableCell cell22 = new TableCell();
TableCell cell23 = new TableCell();

// Добавляем элементы контура в ячейку таблицы
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Добавляем ячейки таблицы к строкам
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Инициализируем объект класса Table и устанавливаем ширину столбцов
Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Добавляем строки таблицы в таблицу
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Инициализировать объект Outline
Outline outline = new Outline();

// Инициализировать объект OutlineElement
OutlineElement outlineElem = new OutlineElement();

// Добавляем таблицу к узлу элемента контура
outlineElem.AppendChildLast(table);

// Добавляем элемент контура в контур
outline.AppendChildLast(outlineElem);

// Добавляем контур к узлу страницы
page.AppendChildLast(outline);

// Добавляем страницу в узел документа
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### Смотрите также

* class [Table](../)
* пространство имен [Aspose.Note](../../table/)
* сборка [Aspose.Note](../../../)


