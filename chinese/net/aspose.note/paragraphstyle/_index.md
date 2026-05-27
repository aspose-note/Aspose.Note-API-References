---
title: "ParagraphStyle 类"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.ParagraphStyle 类。如果在 Styles 集合中没有匹配的 TextStyle 对象，或者此对象未指定所需设置，则使用的文本样式设置"
type: docs
weight: 580
url: /zh/net/aspose.note/paragraphstyle/
---
## ParagraphStyle class

如果在 Styles 集合中没有匹配的 TextStyle 对象，或者此对象未指定所需设置，则使用的文本样式设置。

```csharp
public sealed class ParagraphStyle : Style, IEquatable<ParagraphStyle>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ParagraphStyle](paragraphstyle/)() | 初始化 `ParagraphStyle` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| static [Default](../../aspose.note/paragraphstyle/default/) { get; } | 获取具有默认设置的 ParagraphStyle。 |
| [FontColor](../../aspose.note/style/fontcolor/) { get; set; } | 获取或设置字体颜色。 |
| [FontName](../../aspose.note/style/fontname/) { get; set; } | 获取或设置字体名称。 |
| [FontSize](../../aspose.note/style/fontsize/) { get; set; } | 获取或设置字体大小。 |
| [FontStyle](../../aspose.note/style/fontstyle/) { get; } | 获取字体样式。 |
| [Highlight](../../aspose.note/style/highlight/) { get; set; } | 获取或设置突出显示颜色。 |
| [IsBold](../../aspose.note/style/isbold/) { get; set; } | 获取或设置一个值，指示文本样式是否为粗体。 |
| [IsItalic](../../aspose.note/style/isitalic/) { get; set; } | 获取或设置一个值，指示文本样式是否为斜体。 |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough/) { get; set; } | 获取或设置一个值，指示文本样式是否有删除线。 |
| [IsSubscript](../../aspose.note/style/issubscript/) { get; set; } | 获取或设置一个值，指示文本样式是否为下标。 |
| [IsSuperscript](../../aspose.note/style/issuperscript/) { get; set; } | 获取或设置一个值，指示文本样式是否为上标。 |
| [IsUnderline](../../aspose.note/style/isunderline/) { get; set; } | 获取或设置一个值，指示文本样式是否带下划线。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.note/paragraphstyle/equals/#equals_1)(object) | 确定指定的对象是否等于当前对象。 |
| [Equals](../../aspose.note/paragraphstyle/equals/#equals)(ParagraphStyle) | 确定指定的对象是否等于当前对象。 |
| override [GetHashCode](../../aspose.note/paragraphstyle/gethashcode/)() | 作为该类型的哈希函数。 |

## 示例

让我们通过增大字体大小来强调页面的标题，而不是其他标题。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
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

让我们通过高亮来强调最新文本的更改。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Aspose.one");

// 获取上周修改的 RichText 节点。
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // 设置高亮颜色
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // 设置高亮颜色
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
```

使用段落样式操作文本格式。

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

展示如何插入新的项目符号列表。

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

// 初始化 OutlineElement 类对象并应用项目符号
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };

// 初始化 RichText 类对象并应用文本样式
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(  ) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
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
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
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

* class [Style](../style/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


