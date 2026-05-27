---
title: "类 TableRow"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.TableRow 类。表示一个表格行"
type: docs
weight: 1010
url: /zh/net/aspose.note/tablerow/
---
## TableRow class

表示表格行。

```csharp
public sealed class TableRow : CompositeNode<TableCell>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [TableRow](tablerow/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablerow/lastmodifiedtime/) { get; set; } | 获取或设置最后修改时间。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树层级的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树层级的上一个节点。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/tablerow/accept/)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;TableCell&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params TableCell[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

## 示例

展示如何从每个表格的行中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Sample1.one");

// 获取表格节点列表
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // 遍历表格行
    foreach (TableRow row in table)
    {
        // 检索文本
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // 在输出屏幕上打印文本
        Console.WriteLine(text);
    }
}
```

展示如何从表格的单元格中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Sample1.one");

// 获取表格节点列表
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // 遍历表格行
    foreach (TableRow row in table)
    {
        // 获取 TableCell 节点列表
        // 遍历表格单元格
        foreach (TableCell cell in row)
        {
            // 检索文本
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 在输出屏幕上打印文本
            Console.WriteLine(text);
        }
    }
}
```

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

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [TableCell](../tablecell/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


