---
title: Class Table
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Table сорт. Представляет таблицу.
type: docs
weight: 900
url: /ru/net/aspose.note/table/
---
## Table class

Представляет таблицу.

```csharp
public sealed class Table : CompositeNode<TableRow>, IOutlineElementChildNode, ITaggable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Table](table/#constructor)() | Инициализирует новый экземпляр`Table` класс. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Columns](../../aspose.note/table/columns/) { get; } | Получает столбцы таблицы. |
| [Document](../../aspose.note/node/document/) { get; } | Получает документ узла. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsBordersVisible](../../aspose.note/table/isbordersvisible/) { get; set; } | Получает или задает значение, указывающее, видна ли граница таблицы. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/table/lastmodifiedtime/) { get; set; } | Получает или устанавливает время последнего изменения. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Получает следующий узел на том же уровне дерева узлов. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Получает тип узла. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Получает родительский узел. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Получает предыдущий узел на том же уровне дерева узлов. |
| [Tags](../../aspose.note/table/tags/) { get; } | Получает список всех тегов абзаца. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Accept](../../aspose.note/table/accept/)(DocumentVisitor) | Принимает посетителя узла. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;TableRow&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params TableRow[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Примеры

Показывает, как получить текст из каждой строки таблицы.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tables();

// Загрузите документ в Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Получаем список узлов таблицы
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // Итерация по строкам таблицы
    foreach (TableRow row in table)
    {
        // Получить текст
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // Печать текста на экране вывода
        Console.WriteLine(text);
    }
}
```

Показывает, как получить текст из таблицы.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tables();

// Загрузите документ в Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Получаем список узлов таблицы
IList<Table> nodes = document.GetChildNodes<Table>();

// Установить количество таблиц
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // Получить текст
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // Печать текста на экране вывода
    Console.WriteLine(text);
}
```

Показывает, как получить текст из ячеек таблицы.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tables();

// Загрузите документ в Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// Получаем список узлов таблицы
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // Итерация по строкам таблицы
    foreach (TableRow row in table)
    {
        // Получить список узлов TableCell
        // Итерация по ячейкам таблицы
        foreach (TableCell cell in row)
        {
            // Получить текст
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // Печать текста на экране вывода
            Console.WriteLine(text);
        }
    }
}
```

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

Показывает, как добавить новую таблицу с тегом.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса TableRow
TableRow row = new TableRow(doc);

// Инициализировать объект класса TableCell
TableCell cell = new TableCell(doc);

// Вставляем содержимое ячейки
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// Добавляем ячейку в узел строки
row.AppendChildLast(cell);

// Инициализировать узел таблицы
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// Вставляем узел строки в таблицу
table.AppendChildLast(row);

// Добавляем тег к этому узлу таблицы
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

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
TableRow row1 = new TableRow(doc);

// Инициализируем объект класса TableCell и устанавливаем текстовое содержимое
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// Инициализировать объект класса TableRow
TableRow row2 = new TableRow(doc);

// Инициализируем объект класса TableCell и устанавливаем текстовое содержимое
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// Инициализировать объект класса Table
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// Добавляем строки
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

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
TableRow row1 = new TableRow(doc);

// Инициализировать объекты класса TableCell
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// Добавляем элементы контура в ячейку таблицы
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// Ячейки таблицы в строки
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// Инициализировать объект класса TableRow
TableRow row2 = new TableRow(doc);

// инициализируем объекты класса TableCell
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// Добавляем элементы контура в ячейку таблицы
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// Добавляем ячейки таблицы к строкам
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// Инициализируем объект класса Table и устанавливаем ширину столбцов
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// Добавляем строки таблицы в таблицу
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// Инициализировать объект Outline
Outline outline = new Outline(doc);

// Инициализировать объект OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

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

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [TableRow](../tablerow/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* пространство имен [Aspose.Note](../../aspose.note/)
* сборка [Aspose.Note](../../)


