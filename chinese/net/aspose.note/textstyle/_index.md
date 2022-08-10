---
title: TextStyle
second_title: Aspose.Note for .NET API 参考
description: 指定文本样式
type: docs
weight: 940
url: /zh/net/aspose.note/textstyle/
---
## TextStyle class

指定文本样式。

```csharp
public sealed class TextStyle : Style
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [TextStyle](textstyle)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| static [Default](../../aspose.note/textstyle/default) { get; } | 获取 MS OneNote 中标题文本的默认样式。 |
| static [DefaultMsOneNoteTitleDateStyle](../../aspose.note/textstyle/defaultmsonenotetitledatestyle) { get; } | 获取 MS OneNote 中标题日期的默认样式。 |
| static [DefaultMsOneNoteTitleTextStyle](../../aspose.note/textstyle/defaultmsonenotetitletextstyle) { get; } | 获取 MS OneNote 中标题文本的默认样式。 |
| static [DefaultMsOneNoteTitleTimeStyle](../../aspose.note/textstyle/defaultmsonenotetitletimestyle) { get; } | 获取 MS OneNote 中标题时间的默认样式。 |
| [FontColor](../../aspose.note/style/fontcolor) { get; set; } | 获取或设置字体颜色。 |
| [FontName](../../aspose.note/style/fontname) { get; set; } | 获取或设置字体名称。 |
| [FontSize](../../aspose.note/style/fontsize) { get; set; } | 获取或设置字体大小。 |
| [FontStyle](../../aspose.note/style/fontstyle) { get; } | 获取字体样式。 |
| [Highlight](../../aspose.note/style/highlight) { get; set; } | 获取或设置高亮颜色。 |
| [HyperlinkAddress](../../aspose.note/textstyle/hyperlinkaddress) { get; set; } | 获取或设置超链接地址。如果值为[`IsHyperlink`](./ishyperlink)属性为真。 |
| [IsBold](../../aspose.note/style/isbold) { get; set; } | 获取或设置一个值，指示文本样式是否为粗体。 |
| [IsHidden](../../aspose.note/textstyle/ishidden) { get; set; } | 获取或设置文本样式是否隐藏的值。 |
| [IsHyperlink](../../aspose.note/textstyle/ishyperlink) { get; set; } | 获取或设置文本样式是否为超链接的值。 |
| [IsItalic](../../aspose.note/style/isitalic) { get; set; } | 获取或设置文本样式是否为斜体的值。 |
| [IsMathFormatting](../../aspose.note/textstyle/ismathformatting) { get; set; } | 获取或设置一个值，该值指示文本样式是否为数学格式。 |
| [IsStrikethrough](../../aspose.note/style/isstrikethrough) { get; set; } | 获取或设置一个值，该值指示文本样式是否为删除线。 |
| [IsSubscript](../../aspose.note/style/issubscript) { get; set; } | 获取或设置文本样式是否为下标的值。 |
| [IsSuperscript](../../aspose.note/style/issuperscript) { get; set; } | 获取或设置文本样式是否为上标的值。 |
| [IsUnderline](../../aspose.note/style/isunderline) { get; set; } | 获取或设置文本样式是否为下划线的值。 |
| [Language](../../aspose.note/textstyle/language) { get; set; } | 获取或设置文本的语言。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Equals](../../aspose.note/textstyle/equals#equals_1)(object) | 判断指定对象是否等于当前对象 |
| [Equals](../../aspose.note/textstyle/equals#equals)(TextStyle) | 判断指定对象是否等于当前对象 |
| override [GetHashCode](../../aspose.note/textstyle/gethashcode)() | 用作类型的哈希函数。 |

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

让我们通过突出显示来强调最新文本的变化。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note。
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

设置文本的校对语言。

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

使用段落样式按文本格式进行操作。

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

显示如何将超链接绑定到文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tasks();

// 创建 Document 类的对象
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// 添加轮廓元素
outline.AppendChildLast(outlineElem);

// 初始化 Title 类对象
Title title = new Title() { TitleText = titleText };

//初始化Page类对象
Page page = new Note.Page() { Title = title };

// 添加大纲节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### 也可以看看

* class [Style](../style)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
