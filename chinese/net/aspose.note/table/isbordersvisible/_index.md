---
title: Table.IsBordersVisible
second_title: Aspose.Note for .NET API 参考
description: Table 财产. 获取或设置一个值指示表格边框是否可见
type: docs
weight: 30
url: /zh/net/aspose.note/table/isbordersvisible/
---
## Table.IsBordersVisible property

获取或设置一个值，指示表格边框是否可见。

```csharp
public bool IsBordersVisible { get; set; }
```

### 例子

显示如何为单元格设置背景颜色。

```csharp
// 创建文档类的对象
Document doc = new Document();

// 初始化TableCell类对象并设置文本内容
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// 初始化 TableRow 类对象
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

// 初始化页面类对象
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

显示如何添加带有标签的新表。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 创建文档类的对象
Document doc = new Document();

// 初始化页面类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 TableRow 类对象
TableRow row = new TableRow(doc);

// 初始化 TableCell 类对象
TableCell cell = new TableCell(doc);

//插入单元格内容
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// 将单元格添加到行节点
row.AppendChildLast(cell);

// 初始化表节点
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// 在表中插入行节点
table.AppendChildLast(row);

// 给这个表节点添加标签
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// 添加表节点
outlineElem.AppendChildLast(table);

// 添加轮廓元素
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

显示如何创建具有锁定列的表。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 创建文档类的对象
Document doc = new Document();

// 初始化页面类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 TableRow 类对象
TableRow row1 = new TableRow(doc);

// 初始化TableCell类对象并设置文本内容
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// 初始化 TableRow 类对象
TableRow row2 = new TableRow(doc);

// 初始化TableCell类对象并设置文本内容
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// 初始化表类对象
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// 添加行
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// 添加表节点
outlineElem.AppendChildLast(table);

// 添加轮廓元素节点
outline.AppendChildLast(outlineElem);

// 添加轮廓节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

显示如何创建新表。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 创建文档类的对象
Document doc = new Document();

// 初始化页面类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 TableRow 类对象
TableRow row1 = new TableRow(doc);

// 初始化 TableCell 类对象
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// 在表格单元格中追加轮廓元素
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// 表格单元格到行
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// 初始化 TableRow 类对象
TableRow row2 = new TableRow(doc);

// 初始化 TableCell 类对象
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// 在表格单元格中追加轮廓元素
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// 将表格单元格附加到行
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// 初始化 Table 类对象并设置列宽
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// 将表行追加到表中
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// 初始化轮廓对象
Outline outline = new Outline(doc);

// 初始化 OutlineElement 对象
OutlineElement outlineElem = new OutlineElement(doc);

// 添加表到大纲元素节点
outlineElem.AppendChildLast(table);

// 将轮廓元素添加到轮廓
outline.AppendChildLast(outlineElem);

// 给页面节点添加轮廓
page.AppendChildLast(outline);

// 添加页面到文档节点
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### 也可以看看

* class [Table](../)
* 命名空间 [Aspose.Note](../../table/)
* 部件 [Aspose.Note](../../../)


