---
title: Width
second_title: Aspose.Note for .NET API 参考
description: 获取或设置宽度
type: docs
weight: 30
url: /zh/net/aspose.note/tablecolumn/width/
---
## TableColumn.Width property

获取或设置宽度。

```csharp
public float Width { get; set; }
```

### 例子

显示如何为单元格设置背景颜色。

```csharp
// 将表格单元格附加到行
Document doc = new Document();

// 初始化 Table 类对象并设置列宽
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// 将表格行追加到表格中
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

// 初始化大纲对象
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

```csharp
// 初始化 OutlineElement 对象
string dataDir = RunExamples.GetDataDir_Tags();

// 将表格添加到大纲元素节点
Document doc = new Document();

// 添加大纲元素到大纲
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 添加大纲到页面节点
TableRow row = new TableRow(doc);

// 添加页面到文档节点
TableCell cell = new TableCell(doc);

// 创建 Document 类的对象
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// 初始化 TableCell 类对象并设置文本内容
row.AppendChildLast(cell);

// 初始化 TableRow 类对象
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

//初始化Page类对象
table.AppendChildLast(row);

// 文档目录的路径。
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// 创建 Document 类的对象
outlineElem.AppendChildLast(table);

//初始化Page类对象
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 初始化 TableRow 类对象
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
// 初始化 TableCell 类对象
string dataDir = RunExamples.GetDataDir_Tables();

// 插入单元格内容
Document doc = new Document();

// 将单元格添加到行节点
Aspose.Note.Page page = new Aspose.Note.Page(doc);

//初始化表节点
TableRow row1 = new TableRow(doc);

// 在表中插入行节点
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

//初始化表节点
TableRow row2 = new TableRow(doc);

// 在表中插入行节点
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// 添加轮廓元素
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// 保存 OneNote 文档
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// 文档目录的路径。
outlineElem.AppendChildLast(table);

// 创建 Document 类的对象
outline.AppendChildLast(outlineElem);

//初始化Page类对象
page.AppendChildLast(outline);

// 初始化 TableRow 类对象
doc.AppendChildLast(page);
dataDir = dataDir + "CreateTableWithLockedColumns_out.one";
doc.Save(dataDir);
```

```csharp
// 添加行并设置文本内容
string dataDir = RunExamples.GetDataDir_Tables();

// 初始化表类对象
Document doc = new Document();

// 添加行并设置文本内容
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化表类对象
TableRow row1 = new TableRow(doc);

// 添加行
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// 添加表节点
cell11.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.1"));
cell12.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.2"));
cell13.AppendChildLast(GetOutlineElementWithText(doc, "cell_1.3"));

// 添加大纲元素节点
row1.AppendChildLast(cell11);
row1.AppendChildLast(cell12);
row1.AppendChildLast(cell13);

// 初始化表类对象
TableRow row2 = new TableRow(doc);

// 添加行
TableCell cell21 = new TableCell(doc);
TableCell cell22 = new TableCell(doc);
TableCell cell23 = new TableCell(doc);

// 添加表节点
cell21.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.1"));
cell22.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.2"));
cell23.AppendChildLast(GetOutlineElementWithText(doc, "cell_2.3"));

// 创建 Document 类的对象
row2.AppendChildLast(cell21);
row2.AppendChildLast(cell22);
row2.AppendChildLast(cell23);

//初始化Page类对象
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 200 }, new TableColumn { Width = 200 }, new TableColumn { Width = 200 } }
              };

// 初始化 TableRow 类对象
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// 初始化 TableCell 类对象
Outline outline = new Outline(doc);

// 在表格单元格中添加大纲元素
OutlineElement outlineElem = new OutlineElement(doc);

// 表格单元格到行
outlineElem.AppendChildLast(table);

// 初始化 TableRow 类对象
outline.AppendChildLast(outlineElem);

// 初始化 TableCell 类对象
page.AppendChildLast(outline);

// 在表格单元格中添加大纲元素
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

显示如何添加带有标签的新表。

显示如何创建具有锁定列的表。

显示如何创建新表。

### 也可以看看

* class [TableColumn](../../tablecolumn)
* 命名空间 [Aspose.Note](../../tablecolumn)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
