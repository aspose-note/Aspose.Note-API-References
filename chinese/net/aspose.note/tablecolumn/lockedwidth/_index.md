---
title: TableColumn.LockedWidth
second_title: Aspose.Note for .NET API 参考
description: TableColumn 财产. 获取或设置一个值该值指示表列是否已锁定宽度并且不会自动调整大小以适应表内容 默认情况下列宽未锁定
type: docs
weight: 20
url: /zh/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

获取或设置一个值，该值指示表列是否已锁定宽度并且不会自动调整大小以适应表内容。 默认情况下，列宽未锁定。

```csharp
public bool LockedWidth { get; set; }
```

### 例子

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

### 也可以看看

* class [TableColumn](../)
* 命名空间 [Aspose.Note](../../tablecolumn/)
* 部件 [Aspose.Note](../../../)


