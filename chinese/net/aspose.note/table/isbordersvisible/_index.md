---
title: "Table.IsBordersVisible"
second_title: "Aspose.Note for .NET API 参考"
description: "Table 属性。获取或设置一个指示表格边框是否可见的值"
type: docs
weight: 30
url: /zh/net/aspose.note/table/isbordersvisible/
---
## Table.IsBordersVisible property

获取或设置指示表格边框是否可见的值。

```csharp
public bool IsBordersVisible { get; set; }
```

## 示例

展示如何为单元格设置背景颜色。

```csharp
// 创建 Document 类的对象
Document doc = new Document();

// 初始化 TableCell 类对象并设置文本内容
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText("Small text"));
cell11.BackgroundColor = Color.Coral;

// 初始化 TableRow 类对象
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

// 初始化 Page 类对象
Page page = new Page();
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

展示如何添加带标签的新表格。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 TableRow 类对象
TableRow row = new TableRow();

// 初始化 TableCell 类对象
TableCell cell = new TableCell();

// 插入单元格内容
cell.AppendChildLast(InsertTable.GetOutlineElementWithText("Single cell."));

// 将单元格添加到行节点
row.AppendChildLast(cell);

// 初始化表格节点
Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// 在表格中插入行节点
table.AppendChildLast(row);

// 为此表格节点添加标签
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline();
OutlineElement outlineElem = new OutlineElement();

// 添加表格节点
outlineElem.AppendChildLast(table);

// 添加大纲元素
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

展示如何创建带有锁定列的表格。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 TableRow 类对象
TableRow row1 = new TableRow();

// 初始化 TableCell 类对象并设置文本内容
TableCell cell11 = new TableCell();
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText("Small text"));
row1.AppendChildLast(cell11);

// 初始化 TableRow 类对象
TableRow row2 = new TableRow();

// 初始化 TableCell 类对象并设置文本内容
TableCell cell21 = new TableCell();
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText("Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// 初始化 Table 类对象
Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// 添加行
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline();
OutlineElement outlineElem = new OutlineElement();

// 添加表格节点
outlineElem.AppendChildLast(table);

// 添加大纲元素节点
outline.AppendChildLast(outlineElem);

// 添加大纲节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

展示如何创建新表格。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 TableRow 类对象
TableRow row1 = new TableRow();

// 初始化 TableCell 类对象
TableCell cell11 = new TableCell();
TableCell cell12 = new TableCell();
TableCell cell13 = new TableCell();

// 在表格单元格中追加轮廓元素
cell11.AppendChildLast(GetOutlineElementWithText("cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText("cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText("cell_1.3"));

// 表格单元格到行
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// 初始化 TableRow 类对象
TableRow row2 = new TableRow();

// 初始化 TableCell 类对象
TableCell cell21 = new TableCell();
TableCell cell22 = new TableCell();
TableCell cell23 = new TableCell();

// 在表格单元格中追加轮廓元素
cell21.AppendChildLast(GetOutlineElementWithText("cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText("cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText("cell_2.3"));

// 将表格单元格追加到行
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

// 初始化 Table 类对象并设置列宽
Table table = new Table()
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// 将表格行追加到表格
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// 初始化 Outline 对象
Outline outline = new Outline();

// 初始化 OutlineElement 对象
OutlineElement outlineElem = new OutlineElement();

// 将表格添加到大纲元素节点
outlineElem.AppendChildLast(table);

// 将大纲元素添加到大纲
outline.AppendChildLast(outlineElem);

// 将大纲添加到页面节点
page.AppendChildLast(outline);

// 将页面添加到文档节点
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### 另请参阅

* class [Table](../)
* namespace [Aspose.Note](../../table/)
* assembly [Aspose.Note](../../../)


