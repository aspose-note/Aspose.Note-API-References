---
title: Style.FontName
second_title: Aspose.Note for .NET API 参考
description: Style 财产. 获取或设置字体名称
type: docs
weight: 20
url: /zh/net/aspose.note/style/fontname/
---
## Style.FontName property

获取或设置字体名称。

```csharp
public string FontName { get; set; }
```

### 例子

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

// 同一轮廓内的数字自动递增。
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

显示如何插入新的项目符号列表。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 创建文档类的对象
Aspose.Note.Document doc = new Aspose.Note.Document();

// 初始化页面类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化大纲类对象
Outline outline = new Outline(doc);

// 初始化 TextStyle 类对象并设置格式属性
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 OutlineElement 类对象并应用项目符号
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// 初始化 RichText 类对象并应用文本样式
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 添加轮廓元素
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 添加轮廓节点
page.AppendChildLast(outline);
// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

显示如何插入带有编号的新列表。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 创建文档类的对象
Document doc = new Document();

// 初始化页面类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化大纲类对象
Outline outline = new Outline(doc);

// 初始化 TextStyle 类对象并设置格式属性
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 OutlineElement 类对象并应用编号
// 同一轮廓内的数字自动递增。
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

// 添加轮廓节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

显示如何将超链接绑定到文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tasks();

// 创建文档类的对象
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

// 初始化标题类对象
Title title = new Title() { TitleText = titleText };

// 初始化页面类对象
Page page = new Note.Page() { Title = title };

// 添加轮廓节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### 也可以看看

* class [Style](../)
* 命名空间 [Aspose.Note](../../style/)
* 部件 [Aspose.Note](../../../)


