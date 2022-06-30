---
title: TableRow
second_title: Aspose.Note for .NET API 参考
description: 表示一个表行
type: docs
weight: 900
url: /zh/net/aspose.note/tablerow/
---
## TableRow class

表示一个表行。

```csharp
public sealed class TableRow : CompositeNode<TableCell>
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [TableRow](tablerow#constructor)() | 初始化[`TableRow`](../tablerow)类的新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/tablerow/lastmodifiedtime) { get; set; } | 获取或设置最后修改时间。 |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/tablerow/accept)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;TableCell&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params TableCell[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### 例子

显示如何从每个表的行中获取文本。

```csharp
// 初始化表类对象
string dataDir = RunExamples.GetDataDir_Tables();

// 添加行
Document document = new Document(dataDir + "Sample1.one");

// 添加表节点
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // 添加大纲元素节点
    foreach (TableRow row in table)
    {
        // 添加大纲节点
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // 添加页面节点
        Console.WriteLine(text);
    }
}
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 创建 Document 类的对象
Document document = new Document(dataDir + "Sample1.one");

//初始化Page类对象
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // 初始化 TableRow 类对象
    foreach (TableRow row in table)
    {
        // 初始化 TableCell 类对象
        // 在表格单元格中添加大纲元素
        foreach (TableCell cell in row)
        {
            // 表格单元格到行
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 初始化 TableRow 类对象
            Console.WriteLine(text);
        }
    }
}
```

```csharp
// 初始化 TableCell 类对象
Document doc = new Document();

// 在表格单元格中添加大纲元素
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
cell11.BackgroundColor = Color.Coral;

// 将表格单元格附加到行
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

// 初始化 Table 类对象并设置列宽
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

```csharp
// 将表格行追加到表格中
string dataDir = RunExamples.GetDataDir_Tags();

// 初始化大纲对象
Document doc = new Document();

// 初始化 OutlineElement 对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 将表格添加到大纲元素节点
TableRow row = new TableRow(doc);

// 添加大纲元素到大纲
TableCell cell = new TableCell(doc);

// 添加大纲到页面节点
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// 添加页面到文档节点
row.AppendChildLast(cell);

// 创建 Document 类的对象
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70 } }
              };

// 初始化 TableCell 类对象并设置文本内容
table.AppendChildLast(row);

// 初始化 TableRow 类对象
table.Tags.Add(NoteTag.CreateQuestionMark());

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

//初始化Page类对象
outlineElem.AppendChildLast(table);

// 文档目录的路径。
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 将文档加载到 Aspose.Note。
dataDir = dataDir + "AddTableNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
// 获取表节点列表
string dataDir = RunExamples.GetDataDir_Tables();

// 遍历表行
Document doc = new Document();

// 获取文本
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 在输出屏幕上打印文本
TableRow row1 = new TableRow(doc);

// 文档目录的路径。
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// 在输出屏幕上打印文本
TableRow row2 = new TableRow(doc);

// 文档目录的路径。
TableCell cell21 = new TableCell(doc);
cell21.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Long   text    with    several   words and    spaces."));
row2.AppendChildLast(cell21);

// 遍历表行
Table table = new Table(doc)
              {
                  IsBordersVisible = true,
                  Columns = { new TableColumn { Width = 70, LockedWidth = true } }
              };

// 获取 TableCell 节点列表
table.AppendChildLast(row1);
table.AppendChildLast(row2);

Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);

// 遍历表格单元格
outlineElem.AppendChildLast(table);

// 获取文本
outline.AppendChildLast(outlineElem);

// 在输出屏幕上打印文本
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

显示如何从表格的单元格中获取文本。

显示如何为单元格设置背景颜色。

显示如何添加带有标签的新表。

显示如何创建具有锁定列的表。

显示如何创建新表。

### 也可以看看

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [TableCell](../tablecell)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
