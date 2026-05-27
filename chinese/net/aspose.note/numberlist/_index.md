---
title: "类 NumberList"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.NumberList 类。表示编号或项目符号列表"
type: docs
weight: 510
url: /zh/net/aspose.note/numberlist/
---
## NumberList class

表示编号或项目符号列表。

```csharp
public class NumberList
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [NumberList](numberlist/#constructor_1)(string, string, int) | 初始化 `NumberList` 类的新实例。此实例表示项目符号列表。 |
| [NumberList](numberlist/#constructor)(string, NumberFormat, string, int) | 初始化 `NumberList` 类的新实例。此实例表示编号列表。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Font](../../aspose.note/numberlist/font/) { get; set; } | 获取或设置字体的名称。 |
| [FontColor](../../aspose.note/numberlist/fontcolor/) { get; set; } | 获取或设置字体颜色。 |
| [FontSize](../../aspose.note/numberlist/fontsize/) { get; set; } | 获取或设置字体大小。 |
| [Format](../../aspose.note/numberlist/format/) { get; set; } | 获取或设置行标题的格式。对于项目符号列表，表示项目符号符号。 |
| [IsBold](../../aspose.note/numberlist/isbold/) { get; set; } | 获取或设置一个值，指示文本样式是否为粗体。 |
| [IsItalic](../../aspose.note/numberlist/isitalic/) { get; set; } | 获取或设置一个值，指示文本样式是否为斜体。 |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime/) { get; set; } | 获取或设置最后修改时间。 |
| [NumberFormat](../../aspose.note/numberlist/numberformat/) { get; set; } | 获取或设置用于一组自动编号对象的数字格式。对于项目符号列表应为 null。 |
| [Restart](../../aspose.note/numberlist/restart/) { get; set; } | 获取或设置覆盖列表项自动编号值的数值。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals/#equals)(NumberList) | 确定指定的对象是否等于当前对象。 |
| override [Equals](../../aspose.note/numberlist/equals/#equals_1)(object) | 确定指定的对象是否等于当前对象。 |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode/)() | 作为该类型的哈希函数。 |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader/)(int) | 获取编号列表标题。 |

## 示例

展示如何检索列表格式的信息。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// 检索大纲元素的节点集合
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// 遍历每个节点
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // 检索字体名称
        Console.WriteLine("Font Name: " + list.Font);

        // 检索字体长度
        Console.WriteLine("Font Length: " + list.Font.Length);

        // 检索字体大小
        Console.WriteLine("Font Size: " + list.FontSize);

        // 检索字体颜色
        Console.WriteLine("Font Color: " + list.FontColor);

        // 检索格式
        Console.WriteLine("Font format: " + list.Format);

        // 检查粗体
        Console.WriteLine("Is bold: " + list.IsBold);

        // 检查斜体
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

展示如何插入带中文编号的新列表。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 初始化 OneNote 文档
Document doc = new Document();

// 初始化 OneNote 页面
Page page = new Page();
Outline outline = new Outline();

// 应用文本样式设置
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 同一大纲中的数字会自动递增。
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
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

展示如何插入带编号的新列表。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象
Outline outline = new Outline();

// 初始化 TextStyle 类对象并设置格式属性
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 OutlineElement 类对象并应用编号
// 同一大纲中的数字会自动递增。
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 添加大纲元素
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 添加 Outline 节点
page.AppendChildLast(outline);

// 添加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### 另请参阅

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


