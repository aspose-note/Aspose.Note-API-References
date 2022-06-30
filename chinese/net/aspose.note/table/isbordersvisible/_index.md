---
title: IsBordersVisible
second_title: Aspose.Note for .NET API 参考
description: 获取或设置表格边框是否可见的值
type: docs
weight: 30
url: /zh/net/aspose.note/table/isbordersvisible/
---
## Table.IsBordersVisible property

获取或设置表格边框是否可见的值。

```csharp
public bool IsBordersVisible { get; set; }
```

### 例子

显示如何为单元格设置背景颜色。

```csharp
// 初始化 TableRow 类对象
Document doc = new Document();

// 初始化 TableCell 类对象并设置文本内容
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

// 初始化 TableCell 类对象并设置文本内容
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

```csharp
// 初始化表类对象
string dataDir = RunExamples.GetDataDir_Tags();

// 添加行
Document doc = new Document();

// 初始化 TableCell 类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 添加大纲元素节点
TableRow row = new TableRow(doc);

// 添加大纲节点
TableCell cell = new TableCell(doc);

// 添加页面节点
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// 文档目录的路径。
row.AppendChildLast(cell);

// 创建 Document 类的对象
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

//初始化Page类对象
table.AppendChildLast(row);

// 初始化 TableRow 类对象
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// 初始化 TableCell 类对象
outlineElem.AppendChildLast(table);

// 在表格单元格中添加大纲元素
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 表格单元格到行
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
// 将表格单元格附加到行
string dataDir = RunExamples.GetDataDir_Tables();

// 初始化 TableCell 类对象
Document doc = new Document();

// 在表格单元格中添加大纲元素
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 将表格单元格附加到行
TableRow row1 = new TableRow(doc);

// 初始化 Table 类对象并设置列宽
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// 将表格单元格附加到行
TableRow row2 = new TableRow(doc);

// 初始化 Table 类对象并设置列宽
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// 初始化 OutlineElement 对象
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// 将表格添加到大纲元素节点
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// 添加大纲元素到大纲
outlineElem.AppendChildLast(table);

// 添加大纲到页面节点
outline.AppendChildLast(outlineElem);

// 添加页面到文档节点
page.AppendChildLast(outline);

// 创建 Document 类的对象
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

```csharp
// 创建 Document 类的对象并设置文本内容
string dataDir = RunExamples.GetDataDir_Tables();

// 文档目录的路径。
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 文档目录的路径。
TableRow row1 = new TableRow(doc);

// 创建 Document 类的对象
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

//初始化Page类对象
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// 插入单元格内容
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// 文档目录的路径。
TableRow row2 = new TableRow(doc);

// 创建 Document 类的对象
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

//初始化Page类对象
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

//初始化表节点
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// 在表中插入行节点
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// 给这个表节点添加标签
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// 添加表节点
Outline outline = new Outline(doc);

// 添加轮廓元素
OutlineElement outlineElem = new OutlineElement(doc);

// 保存 OneNote 文档
outlineElem.AppendChildLast(table);

// 文档目录的路径。
outline.AppendChildLast(outlineElem);

// 创建 Document 类的对象
page.AppendChildLast(outline);

//初始化Page类对象
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

显示如何添加带有标签的新表。

显示如何创建具有锁定列的表。

显示如何创建新表。

### 也可以看看

* class [Table](../../table)
* 命名空间 [Aspose.Note](../../table)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
