---
title: "TableCell.BackgroundColor"
second_title: "Aspose.Note for .NET API 参考"
description: "TableCell 属性。获取或设置背景颜色"
type: docs
weight: 20
url: /zh/net/aspose.note/tablecell/backgroundcolor/
---
## TableCell.BackgroundColor property

获取或设置背景颜色。

```csharp
public Color BackgroundColor { get; set; }
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

### 另请参阅

* class [TableCell](../)
* namespace [Aspose.Note](../../tablecell/)
* assembly [Aspose.Note](../../../)


