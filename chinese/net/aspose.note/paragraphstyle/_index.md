---
title: ParagraphStyle
second_title: Aspose.Note for .NET API 参考
description: 如果在Styles集合中没有匹配的 TextStyle 对象则使用文本样式设置或此对象没有指定需要的设置
type: docs
weight: 490
url: /zh/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

如果在Styles集合中没有匹配的 TextStyle 对象，则使用文本样式设置或此对象没有指定需要的设置。

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [ParagraphStyle](paragraphstyle)() | 初始化[`ParagraphStyle`](../paragraphstyle)类的新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default) { get; } | 使用默认设置获取 ParagraphStyle。 |
| [FontColor](../../aspose.note/style/fontcolor) { get; set; } | 获取或设置字体颜色。 |
| [FontName](../../aspose.note/style/fontname) { get; set; } | 获取或设置字体名称。 |
| [FontSize](../../aspose.note/style/fontsize) { get; set; } | 获取或设置字体大小。 |
| [FontStyle](../../aspose.note/style/fontstyle) { get; } | 获取字体样式。 |
| [Highlight](../../aspose.note/style/highlight) { get; set; } | 获取或设置高亮颜色。 |
| [IsBold](../../aspose.note/style/isbold) { get; set; } | 获取或设置一个值，指示文本样式是否为粗体。 |
| [IsItalic](../../aspose.note/style/isitalic) { get; set; } | 获取或设置一个值，指示文本样式是否为斜体。 |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough) { get; set; } | 获取或设置一个值，该值指示文本样式是否为删除线。 |
| [IsSubscript](../../aspose.note/style/issubscript) { get; set; } | 获取或设置一个值，该值指示文本样式是否为下标。 |
| [IsSuperscript](../../aspose.note/style/issuperscript) { get; set; } | 获取或设置一个值，指示文本样式是否为上标。 |
| [IsUnderline](../../aspose.note/style/isunderline) { get; set; } | 获取或设置一个值，指示文本样式是否为下划线。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals#equals_1)(object) | 判断指定对象是否等于当前对象。 |
| [Equals](../../aspose.note/paragraphstyle/equals#equals)(ParagraphStyle) | 判断指定对象是否等于当前对象。 |
| override [GetHashCode](../../aspose.note/style/gethashcode)() | 用作该类型的哈希函数。 |

### 例子

让我们通过增加字体大小来在其他标题中强调页面标题。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note。
Document document = new Document(dataDir + "Aspose.one");

// 遍历页面的标题。
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

的头衔。
Document document = new Document(dataDir + "Aspose.one");

// 将文档加载到 Aspose.Note。
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // 获取上周修改的 RichText 节点。
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // 获取上周修改的 RichText 节点。
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 设置高亮颜色
Aspose.Note.Document doc = new Aspose.Note.Document();

// 初始化 OneNote 文档
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 初始化 OneNote 页面
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 应用文本样式设置
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

// 同一大纲中的数字会自动递增。
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

// 同一大纲中的数字会自动递增。
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 同一大纲中的数字会自动递增。
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

//------------------------
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 添加页面节点
Aspose.Note.Document doc = new Aspose.Note.Document();

// 创建 Document 类的对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

//初始化Page类对象
Outline outline = new Outline(doc);

// 初始化大纲类对象
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 TextStyle 类对象并设置格式属性
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// 初始化 OutlineElement 类对象并应用项目符号
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 初始化 RichText 类对象并应用文本样式
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 添加轮廓元素
page.AppendChildLast(outline);
// 添加大纲节点
doc.AppendChildLast(page);

// 添加页面节点
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 添加页面节点
Document doc = new Document();

// 创建 Document 类的对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

//初始化Page类对象
Outline outline = new Outline(doc);

// 初始化大纲类对象
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 TextStyle 类对象并设置格式属性
// 初始化 OutlineElement 类对象并应用编号
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 同一大纲中的数字会自动递增。
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 添加轮廓元素
page.AppendChildLast(outline);

// 添加大纲节点
doc.AppendChildLast(page);

// 添加页面节点
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

让我们通过突出显示来强调最新文本的更改。

使用段落样式按文本格式进行操作。

显示如何插入带有中文编号的新列表。

显示如何插入新的项目符号列表。

显示如何插入带有编号的新列表。

### 也可以看看

* class [Style](../style)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
