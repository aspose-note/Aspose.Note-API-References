---
title: RichText.Text
second_title: Aspose.Note for .NET API 参考
description: RichText 财产. 获取或设置文本该字符串不得包含任何值为 10换行的字符
type: docs
weight: 100
url: /zh/net/aspose.note/richtext/text/
---
## RichText.Text property

获取或设置文本。该字符串不得包含任何值为 10（换行）的字符。

```csharp
public string Text { get; set; }
```

### 例子

显示如何从文档中获取所有文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 检索文本
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// 在输出屏幕上打印文本
Console.WriteLine(text);
```

显示如何从页面获取所有文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取页面节点列表
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // 检索文本
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // 在输出屏幕上打印文本
    Console.WriteLine(text);
}
```

显示如何从每个表的行中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Sample1.one");

// 获取表节点列表
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    //遍历表行
    foreach (TableRow row in table)
    {
        // 检索文本
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // 在输出屏幕上打印文本
        Console.WriteLine(text);
    }
}
```

演示如何从表中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Sample1.one");

// 获取表节点列表
IList<Table> nodes = document.GetChildNodes<Table>();

// 设置表数
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // 检索文本
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // 在输出屏幕上打印文本
    Console.WriteLine(text);
}
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

显示如何遍历所有页面并在文本中进行替换。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 获取所有 RichText 节点
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 替换形状的文本
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// 保存为任何支持的文件格式
oneFile.Save(dataDir, SaveFormat.Pdf);
```

演示如何从表格的单元格中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Sample1.one");

// 获取表节点列表
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    //遍历表行
    foreach (TableRow row in table)
    {
        // 获取 TableCell 节点列表
        //遍历表格单元格
        foreach (TableCell cell in row)
        {
            // 检索文本
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 在输出屏幕上打印文本
            Console.WriteLine(text);
        }
    }
}
```

显示如何使用默认选项创建文档并将其保存为 html 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化 OneNote 文档
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// 文档中所有文本的默认样式。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// 保存成HTML格式
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
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

显示如何创建文档并以 html 格式保存指定范围的页面。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化 OneNote 文档
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 文档中所有文本的默认样式。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 保存成HTML格式
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
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

显示如何创建带有文本的文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 创建文档类的对象
Document doc = new Document();

// 初始化页面类对象
Page page = new Page(doc);

// 初始化大纲类对象
Outline outline = new Outline(doc);

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement(doc);

// 初始化 TextStyle 类对象并设置格式属性
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 RichText 类对象并应用文本样式
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// 添加 RichText 节点
outlineElem.AppendChildLast(text);

// 添加 OutlineElement 节点
outline.AppendChildLast(outlineElem);

// 添加轮廓节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
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

* class [RichText](../)
* 命名空间 [Aspose.Note](../../richtext/)
* 部件 [Aspose.Note](../../../)


