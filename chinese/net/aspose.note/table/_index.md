---
title: Table
second_title: Aspose.Note for .NET API 参考
description: 表示一个表
type: docs
weight: 870
url: /zh/net/aspose.note/table/
---
## Table class

表示一个表。

```csharp
public sealed class Table : CompositeNode<TableRow>, IOutlineElementChildNode, ITaggable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Table](table#constructor)() | 初始化[`Table`](../table)类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Columns](../../aspose.note/table/columns) { get; } | 获取表的列。 |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [IsBordersVisible](../../aspose.note/table/isbordersvisible) { get; set; } | 获取或设置表格边框是否可见的值。 |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [LastModifiedTime](../../aspose.note/table/lastmodifiedtime) { get; set; } | 获取或设置上次修改时间。 |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |
| [Tags](../../aspose.note/table/tags) { get; } | 获取段落的所有标签列表。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/table/accept)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;TableRow&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params TableRow[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |

### 例子

显示如何从每个表的行中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note。
Document document = new Document(dataDir + "Sample1.one");

// 获取表节点列表
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // 遍历表行
    foreach (TableRow row in table)
    {
        // 获取文本
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // 在输出屏幕上打印文本
        Console.WriteLine(text);
    }
}
```

显示如何从表格中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note。
Document document = new Document(dataDir + "Sample1.one");

// 获取表节点列表
IList<Table> nodes = document.GetChildNodes<Table>();

// 设置表数
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // 获取文本
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // 在输出屏幕上打印文本
    Console.WriteLine(text);
}
```

显示如何从表格的单元格中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note。
Document document = new Document(dataDir + "Sample1.one");

// 获取表节点列表
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // 遍历表行
    foreach (TableRow row in table)
    {
        // 获取 TableCell 节点列表
        // 遍历表格单元格
        foreach (TableCell cell in row)
        {
            // 获取文本
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 在输出屏幕上打印文本
            Console.WriteLine(text);
        }
    }
}
```

显示如何为单元格设置背景颜色。

```csharp
// 创建 Document 类的对象
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

//初始化Page类对象
Page page = new Page(doc);
page.AppendChildLast(o);

doc.AppendChildLast(page);

doc.Save(Path.Combine(RunExamples.GetDataDir_Tables(), "SettingCellBackGroundColor.pdf"));
```

显示如何添加带有标签的新表。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 TableRow 类对象
TableRow row = new TableRow(doc);

// 初始化 TableCell 类对象
TableCell cell = new TableCell(doc);

// 插入单元格内容
cell.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Single cell."));

// 将单元格添加到行节点
row.AppendChildLast(cell);

//初始化表节点
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

演示如何创建具有锁定列的表。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 TableRow 类对象
TableRow row1 = new TableRow(doc);

// 初始化 TableCell 类对象并设置文本内容
TableCell cell11 = new TableCell(doc);
cell11.AppendChildLast(InsertTable.GetOutlineElementWithText(doc, "Small text"));
row1.AppendChildLast(cell11);

// 初始化 TableRow 类对象
TableRow row2 = new TableRow(doc);

// 初始化 TableCell 类对象并设置文本内容
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

// 添加大纲元素节点
outline.AppendChildLast(outlineElem);

// 添加大纲节点
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

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 TableRow 类对象
TableRow row1 = new TableRow(doc);

// 初始化 TableCell 类对象
TableCell cell11 = new TableCell(doc);
TableCell cell12 = new TableCell(doc);
TableCell cell13 = new TableCell(doc);

// 在表格单元格中添加大纲元素
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

// 在表格单元格中添加大纲元素
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

// 将表格行追加到表格中
table.AppendChildLast(row1);
table.AppendChildLast(row2);

// 初始化大纲对象
Outline outline = new Outline(doc);

// 初始化 OutlineElement 对象
OutlineElement outlineElem = new OutlineElement(doc);

// 将表格添加到大纲元素节点
outlineElem.AppendChildLast(table);

// 添加大纲元素到大纲
outline.AppendChildLast(outlineElem);

// 添加大纲到页面节点
page.AppendChildLast(outline);

// 添加页面到文档节点
doc.AppendChildLast(page);
dataDir = dataDir + "InsertTable_out.one";
doc.Save(dataDir);
```

### 也可以看看

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [TableRow](../tablerow)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [ITaggable](../itaggable)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
