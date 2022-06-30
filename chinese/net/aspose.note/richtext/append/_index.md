---
title: Append
second_title: Aspose.Note for .NET API 参考
description: 在末尾添加一个字符串
type: docs
weight: 130
url: /zh/net/aspose.note/richtext/append/
---
## Append(string, TextStyle) {#append_1}

在末尾添加一个字符串。

```csharp
public RichText Append(string value, TextStyle style)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| value | String | 附加值。 |
| style | TextStyle | 添加字符串的样式。 |

### 返回值

[`RichText`](../../richtext)。

### 例子

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
// 初始化 TextStyle 类对象并设置格式属性
string dataDir = RunExamples.GetDataDir_Tasks();

// 初始化 OutlineElement 类对象并应用编号
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

// 同一大纲中的数字会自动递增。
outline.AppendChildLast(outlineElem);

// 添加轮廓元素
Title title = new Title() { TitleText = titleText };

// 文档目录的路径。
Page page = new Note.Page() { Title = title };

// 文档目录的路径。
page.AppendChildLast(outline);

// 文档目录的路径。
doc.AppendChildLast(page);

// 文档目录的路径。
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document doc = new Document();

// 创建 Document 类的对象
Page page = new Page();

// 添加轮廓元素
Title title = new Title();

// 初始化 Title 类对象
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

//初始化Page类对象
page.Title = title;

// 让我们添加一组列和一个标题行
outlineElem.AppendChildLast(text);

// 表格前的摘要文本
outline.AppendChildLast(outlineElem);

// 让我们添加一组列和一个标题行
page.AppendChildLast(outline);

// 表格前的摘要文本
doc.AppendChildLast(page);

// 让我们添加一组列和一个标题行
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

使用段落样式按文本格式进行操作。

显示如何将超链接绑定到文本。

展示如何使用格式化的富文本创建文档。

### 也可以看看

* class [TextStyle](../../textstyle)
* class [RichText](../../richtext)
* 命名空间 [Aspose.Note](../../richtext)
* 部件 [Aspose.Note](../../../)

---

## Append(string) {#append}

将字符串添加到最后一个文本范围。

```csharp
public RichText Append(string value)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| value | String | 附加值。 |

### 返回值

[`RichText`](../../richtext)。

### 例子

使用段落样式按文本格式操作。

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
// 让我们 5 个空行。行具有互换的背景颜色
string dataDir = RunExamples.GetDataDir_Tasks();

// 让我们为“联系人”列中的内容添加一些模板
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

添加一组列和一个标题行
outline.AppendChildLast(outlineElem);

5 个空行。行具有互换的背景颜色
Title title = new Title() { TitleText = titleText };

// 文档目录的路径。
Page page = new Note.Page() { Title = title };

// 将文档加载到 Aspose.Note。
page.AppendChildLast(outline);

// 获取所有富文本节点
doc.AppendChildLast(page);

// 遍历每个节点
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

显示如何将超链接绑定到文本。

### 也可以看看

* class [RichText](../../richtext)
* 命名空间 [Aspose.Note](../../richtext)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
