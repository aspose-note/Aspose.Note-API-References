---
title: RichText.ParagraphStyle
second_title: Aspose.Note for .NET API 参考
description: RichText 财产. 获取或设置段落样式 如果在中没有匹配的 TextStyle 对象则使用这些设置Styles收集此对象未指定所需的设置
type: docs
weight: 60
url: /zh/net/aspose.note/richtext/paragraphstyle/
---
## RichText.ParagraphStyle property

获取或设置段落样式。 如果在中没有匹配的 TextStyle 对象，则使用这些设置Styles收集此对象未指定所需的设置。

```csharp
public ParagraphStyle ParagraphStyle { get; set; }
```

### 例子

让我们通过增加字体大小在其他标题中强调页面的标题。

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

展示如何将深色主题样式应用于文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

让我们通过突出显示来强调最新文本的更改。

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

显示如何为页面设置标题。

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
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

显示如何添加带有标签的新段落。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 创建文档类的对象
Document doc = new Document();

// 初始化页面类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化大纲类对象
Outline outline = new Outline(doc);

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// 添加文本节点
outlineElem.AppendChildLast(text);

// 添加轮廓元素节点
outline.AppendChildLast(outlineElem);

// 添加轮廓节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

显示如何访问标签的详细信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "TagFile.one");

// 获取所有 RichText 节点
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

//遍历每个节点
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // 检索属性
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
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

展示如何为每周会议准备模板。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 创建文档类的对象
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
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

* class [ParagraphStyle](../../paragraphstyle/)
* class [RichText](../)
* 命名空间 [Aspose.Note](../../richtext/)
* 部件 [Aspose.Note](../../../)


