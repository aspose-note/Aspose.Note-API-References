---
title: "TableColumn.LockedWidth"
second_title: "Aspose.Note for .NET API 参考"
description: "TableColumn 属性。获取或设置一个值，指示表列是否锁定宽度且不会自动调整以适应表内容。默认情况下列宽未锁定。"
type: docs
weight: 20
url: /zh/net/aspose.note/tablecolumn/lockedwidth/
---
## TableColumn.LockedWidth property

获取或设置一个值，指示表格列是否具有锁定宽度且不会自动调整以适应表格内容。默认情况下，列宽未锁定。

```csharp
public bool LockedWidth { get; set; }
```

## 示例

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

### 另请参阅

* class [TableColumn](../)
* namespace [Aspose.Note](../../tablecolumn/)
* assembly [Aspose.Note](../../../)


