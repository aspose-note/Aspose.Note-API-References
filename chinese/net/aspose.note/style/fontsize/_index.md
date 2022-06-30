---
title: FontSize
second_title: Aspose.Note for .NET API 参考
description: 获取或设置字体大小
type: docs
weight: 30
url: /zh/net/aspose.note/style/fontsize/
---
## Style.FontSize property

获取或设置字体大小。

```csharp
public int? FontSize { get; set; }
```

### 例子

显示如何更改文本的样式。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 添加页面节点
Document document = new Document(dataDir + "Aspose.one");

// 保存 OneNote 文档
RichText richText = document.GetChildNodes<RichText>().First();

foreach (var run in richText.TextRuns)
{
    // 将文档加载到 Aspose.Note。
    run.Style.FontColor = Color.Yellow;

    // 获取特定的 RichText 节点
    run.Style.Highlight = Color.Blue;

    // 设置字体颜色
    run.Style.FontSize = 20;
}
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 设置高亮颜色
Document document = new Document(dataDir + "Aspose.one");

// 设置字体大小
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

// 将文档加载到 Aspose.Note。
Document document = new Document(dataDir + "Aspose.one");

// 遍历页面的标题。
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    的头衔。
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        的头衔。
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

// 获取上周修改的 RichText 节点。
Aspose.Note.Document doc = new Aspose.Note.Document();

// 设置高亮颜色
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 设置高亮颜色
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 OneNote 文档
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

// 初始化 OneNote 页面
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

// 初始化 OneNote 页面
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 初始化 OneNote 页面
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

//------------------------
Aspose.Note.Document doc = new Aspose.Note.Document();

//------------------------
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 添加轮廓元素
Outline outline = new Outline(doc);

// 创建 Document 类的对象
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

//初始化Page类对象
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// 初始化大纲类对象
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 初始化 TextStyle 类对象并设置格式属性
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 初始化 OutlineElement 类对象并应用项目符号
page.AppendChildLast(outline);
// 初始化 RichText 类对象并应用文本样式
doc.AppendChildLast(page);

// 添加轮廓元素
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 初始化 OutlineElement 类对象并应用编号
Document doc = new Document();

// 同一大纲中的数字会自动递增。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 添加轮廓元素
Outline outline = new Outline(doc);

// 创建 Document 类的对象
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

//初始化Page类对象
// 初始化大纲类对象
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 初始化 TextStyle 类对象并设置格式属性
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 初始化 OutlineElement 类对象并应用编号
page.AppendChildLast(outline);

// 同一大纲中的数字会自动递增。
doc.AppendChildLast(page);

// 添加轮廓元素
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
// 添加轮廓元素
string dataDir = RunExamples.GetDataDir_Tasks();

// 初始化 Title 类对象
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

//初始化Page类对象
outline.AppendChildLast(outlineElem);

// 文档目录的路径。
Title title = new Title() { TitleText = titleText };

// 创建 Document 类的对象
Page page = new Note.Page() { Title = title };

// 添加轮廓元素
page.AppendChildLast(outline);

// 初始化 Title 类对象
doc.AppendChildLast(page);

//初始化Page类对象
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var headerText = new RichText() { ParagraphStyle = new ParagraphStyle() { FontSize = 18, IsBold = true }, Alignment = HorizontalAlignment.Center }
                    .Append("Super contest for suppliers.");

var page = new Page();
var outline = page.AppendChildLast(new Outline() { HorizontalOffset = 50 });
outline.AppendChildLast(new OutlineElement()).AppendChildLast(headerText);

// 添加大纲节点
var bodyTextHeader = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
bodyTextHeader.Append("This is the final ranking of proposals got from our suppliers.");

var ranking = outline.AppendChildLast(new OutlineElement()).AppendChildLast(new Table());
var headerRow = ranking.AppendChildFirst(new TableRow());

var headerStyle = ParagraphStyle.Default;
headerStyle.IsBold = true;

// 添加页面节点
var backGroundColor = Color.LightGray;
foreach (var header in new[] { "Supplier", "Contacts", "Score A", "Score B", "Score C", "Final score", "Attached materials", "Comments" })
{
    ranking.Columns.Add(new TableColumn());
    headerRow.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
             .AppendChildLast(new OutlineElement())
             .AppendChildLast(new RichText() { ParagraphStyle = headerStyle })
                .Append(header);
}

// 保存 OneNote 文档
for (int i = 0; i < 5; i++)
{
    backGroundColor = backGroundColor.IsEmpty ? Color.LightGray : Color.Empty;

    var row = ranking.AppendChildLast(new TableRow());
    for (int j = 0; j < ranking.Columns.Count(); j++)
    {
        row.AppendChildLast(new TableCell() { BackgroundColor = backGroundColor })
           .AppendChildLast(new OutlineElement())
           .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default });
    }
}

// 表格前的摘要文本
foreach (var row in ranking.Skip(1))
{
    var contactsCell = row.ElementAt(1);
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("Web: ").Append("link", new TextStyle() { HyperlinkAddress = "www.link.com", IsHyperlink = true });
    contactsCell.AppendChildLast(new OutlineElement())
                .AppendChildLast(new RichText() { ParagraphStyle = ParagraphStyle.Default })
                    .Append("E-mail: ").Append("mail", new TextStyle() { HyperlinkAddress = "mailto:hi@link.com", IsHyperlink = true });
}

var d = new Document();
d.AppendChildLast(page);
d.Save(Path.Combine(dataDir, "ComposeTable_out.one"));
```

让我们通过增加字体大小在其他标题中强调页面标题。

让我们通过突出显示来强调最新文本的更改。

使用段落样式按文本格式进行操作。

显示如何插入带有中文编号的新列表。

显示如何插入新的项目符号列表。

显示如何插入带有编号的新列表。

显示如何将超链接绑定到文本。

展示了如何组合具有各种样式的文本的表格。

### 也可以看看

* class [Style](../../style)
* 命名空间 [Aspose.Note](../../style)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
