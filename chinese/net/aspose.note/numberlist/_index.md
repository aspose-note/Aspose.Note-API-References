---
title: NumberList
second_title: Aspose.Note for .NET API 参考
description: 表示编号或项目符号列表
type: docs
weight: 420
url: /zh/net/aspose.note/numberlist/
---
## NumberList class

表示编号或项目符号列表。

```csharp
public class NumberList
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [NumberList](numberlist#constructor_1)(string, string, int) | 初始化[`NumberList`](../numberlist) class. 这个实例代表一个项目符号列表。 |
| [NumberList](numberlist#constructor)(string, NumberFormat, string, int) | 初始化[`NumberList`](../numberlist)class. 这个实例代表一个编号列表。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Font](../../aspose.note/numberlist/font) { get; set; } | 获取或设置字体名称。 |
| [FontColor](../../aspose.note/numberlist/fontcolor) { get; set; } | 获取或设置字体颜色。 |
| [FontSize](../../aspose.note/numberlist/fontsize) { get; set; } | 获取或设置字体大小。 |
| [Format](../../aspose.note/numberlist/format) { get; set; } | 获取或设置行头的格式。对于项目符号列表代表一个项目符号。 |
| [IsBold](../../aspose.note/numberlist/isbold) { get; set; } | 获取或设置一个值，指示文本样式是否为粗体。 |
| [IsItalic](../../aspose.note/numberlist/isitalic) { get; set; } | 获取或设置文本样式是否为斜体的值。 |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime) { get; set; } | 获取或设置上次修改时间。 |
| [NumberFormat](../../aspose.note/numberlist/numberformat) { get; set; } | 获取或设置用于一组自动编号对象的数字格式。对于项目符号列表应该为空。 |
| [Restart](../../aspose.note/numberlist/restart) { get; set; } | 获取或设置覆盖列表项自动数值的数值。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals#equals)(NumberList) | 判断指定对象是否等于当前对象 |
| override [Equals](../../aspose.note/numberlist/equals#equals_1)(object) | 判断指定对象是否等于当前对象 |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode)() | 用作类型的哈希函数。 |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader)(int) | 获取编号列表头。 |

### 例子

显示如何检索有关列表格式的信息。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// 获取大纲元素的集合节点
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// 遍历每个节点
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // 获取字体名称
        Console.WriteLine("Font Name: " + list.Font);

        // 获取字体长度
        Console.WriteLine("Font Length: " + list.Font.Length);

        // 获取字体大小
        Console.WriteLine("Font Size: " + list.FontSize);

        // 获取字体颜色
        Console.WriteLine("Font Color: " + list.FontColor);

        // 获取格式
        Console.WriteLine("Font format: " + list.Format);

        // 检查粗体
        Console.WriteLine("Is bold: " + list.IsBold);

        // 检查斜体
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

显示如何插入带有中文编号的新列表。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 初始化 OneNote 文档
Aspose.Note.Document doc = new Aspose.Note.Document();

// 初始化 OneNote 页面
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 应用文本样式设置
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 同一大纲中的数字会自动递增。
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

显示如何插入带有编号的新列表。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 创建 Document 类的对象
Document doc = new Document();

//初始化Page类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化大纲类对象
Outline outline = new Outline(doc);

// 初始化 TextStyle 类对象并设置格式属性
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 OutlineElement 类对象并应用编号
// 同一大纲中的数字会自动递增。
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 添加轮廓元素
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 添加大纲节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### 也可以看看

* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
