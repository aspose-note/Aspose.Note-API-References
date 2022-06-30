---
title: Text
second_title: Aspose.Note for .NET API 参考
description: 获取或设置文本字符串不得包含任何值为 10 的字符换行
type: docs
weight: 100
url: /zh/net/aspose.note/richtext/text/
---
## RichText.Text property

获取或设置文本。字符串不得包含任何值为 10 的字符（换行）。

```csharp
public string Text { get; set; }
```

### 例子

显示如何从文档中获取所有文本。

```csharp
// 保存 OneNote 文档
string dataDir = RunExamples.GetDataDir_Text();

// 创建 Document 类的对象
Document oneFile = new Document(dataDir + "Aspose.one");

//初始化Page类对象
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// 初始化大纲类对象
Console.WriteLine(text);
```

```csharp
// 初始化 TextStyle 类对象并设置格式属性
string dataDir = RunExamples.GetDataDir_Text();

// 初始化 OutlineElement 类对象并应用编号
Document oneFile = new Document(dataDir + "Aspose.one");

// 同一大纲中的数字会自动递增。
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // 添加轮廓元素
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // 添加大纲节点
    Console.WriteLine(text);
}
```

```csharp
// 添加页面节点
string dataDir = RunExamples.GetDataDir_Tables();

// 保存 OneNote 文档
Document document = new Document(dataDir + "Sample1.one");

// 文档目录的路径。
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // 创建 Document 类的对象
    foreach (TableRow row in table)
    {
        // 文档目录的路径。
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // 创建 Document 类的对象
        Console.WriteLine(text);
    }
}
```

```csharp
// 添加轮廓元素
string dataDir = RunExamples.GetDataDir_Tables();

// 初始化 Title 类对象
Document document = new Document(dataDir + "Sample1.one");

//初始化Page类对象
IList<Table> nodes = document.GetChildNodes<Table>();

// 添加大纲节点
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // 添加页面节点
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // 保存 OneNote 文档
    Console.WriteLine(text);
}
```

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

```csharp
// 获取上周修改的 RichText 节点。
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// 获取上周修改的 RichText 节点。
Document oneFile = new Document(dataDir + "Aspose.one");

// 设置高亮颜色
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 设置高亮颜色
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// 文档目录的路径。
oneFile.Save(dataDir, SaveFormat.Pdf);
```

```csharp
// 获取文本
string dataDir = RunExamples.GetDataDir_Tables();

// 获取文本
Document document = new Document(dataDir + "Sample1.one");

// 在输出屏幕上打印文本
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // 文档目录的路径。
    foreach (TableRow row in table)
    {
        // 将文档加载到 Aspose.Note。
        // 获取页面节点列表
        foreach (TableCell cell in row)
        {
            // 获取文本
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 在输出屏幕上打印文本
            Console.WriteLine(text);
        }
    }
}
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// 获取表节点列表
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// 遍历表行
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

```csharp
// 获取文本
string dataDir = RunExamples.GetDataDir_Tags();

// 在输出屏幕上打印文本
Document doc = new Document();

// 文档目录的路径。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 将文档加载到 Aspose.Note。
Outline outline = new Outline(doc);

// 获取表节点列表
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// 设置表数
outlineElem.AppendChildLast(text);

// 获取文本
outline.AppendChildLast(outlineElem);

// 在输出屏幕上打印文本
page.AppendChildLast(outline);

// 文档目录的路径。
doc.AppendChildLast(page);

// 将文档加载到 Aspose.Note。
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
// 获取所有富文本节点
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 替换形状的文本
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 保存为任何支持的文件格式
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 文档目录的路径。
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

```csharp
// 获取表节点列表
string dataDir = RunExamples.GetDataDir_Tags();

// 获取表节点列表
Document oneFile = new Document(dataDir + "TagFile.one");

// 遍历表行
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 获取 TableCell 节点列表
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // 遍历表格单元格
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

```csharp
// 获取文本
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 在输出屏幕上打印文本
Document doc = new Document();

// 文档目录的路径。
Page page = new Page(doc);

// 初始化 OneNote 文档
Outline outline = new Outline(doc);

// 文档中所有文本的默认样式。
OutlineElement outlineElem = new OutlineElement(doc);

// 保存为 HTML 格式
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 文档目录的路径。
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// 创建 Document 类的对象
outlineElem.AppendChildLast(text);

//初始化Page类对象
outline.AppendChildLast(outlineElem);

// 初始化大纲类对象
page.AppendChildLast(outline);

// 初始化 OutlineElement 类对象
doc.AppendChildLast(page);

// 添加文本节点
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 添加大纲元素节点
Aspose.Note.Document doc = new Aspose.Note.Document();

// 添加大纲节点
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 添加页面节点
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 保存为 HTML 格式
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

// 文档目录的路径。
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

// 文档目录的路径。
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 文档目录的路径。
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 保存为 HTML 格式
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 文档目录的路径。
Aspose.Note.Document doc = new Aspose.Note.Document();

// 将文档加载到 Aspose.Note。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 获取所有富文本节点
Outline outline = new Outline(doc);

// 遍历每个节点
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 获取属性
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// 文档目录的路径。
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 创建 Document 类的对象
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

//初始化Page类对象
page.AppendChildLast(outline);
// 初始化大纲类对象
doc.AppendChildLast(page);

// 初始化 OutlineElement 类对象
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 添加 OutlineElement 节点
Document doc = new Document();

// 初始化 RichText 类对象并应用文本样式
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 添加富文本节点
Outline outline = new Outline(doc);

// 添加 OutlineElement 节点
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 OneNote 文档
// 初始化 OneNote 页面
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 应用文本样式设置
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 初始化 OneNote 文档
page.AppendChildLast(outline);

// 初始化 OneNote 页面
doc.AppendChildLast(page);

// 应用文本样式设置
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
// 同一大纲中的数字会自动递增。
string dataDir = RunExamples.GetDataDir_Tags();

//------------------------
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

```csharp
//------------------------
string dataDir = RunExamples.GetDataDir_Tasks();

//------------------------
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

// 初始化 OutlineElement 类对象并应用项目符号
outline.AppendChildLast(outlineElem);

// 创建 Document 类的对象
Title title = new Title() { TitleText = titleText };

//初始化Page类对象
Page page = new Note.Page() { Title = title };

// 初始化大纲类对象
page.AppendChildLast(outline);

// 初始化 TextStyle 类对象并设置格式属性
doc.AppendChildLast(page);

// 初始化 OutlineElement 类对象并应用项目符号
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

显示如何从页面获取所有文本。

显示如何从每个表的行中获取文本。

显示如何从表中获取文本。

显示如何为页面设置标题。

显示如何通过所有页面并在文本中进行替换。

显示如何从表格的单元格中获取文本。

显示如何使用默认选项创建文档并将其保存为 html 格式。

显示如何添加带有标签的新段落。

显示如何创建文档并以 html 格式保存指定范围的页面。

显示如何访问标签的详细信息。

显示如何创建带有文本的文档。

显示如何插入带有中文编号的新列表。

显示如何插入新的项目符号列表。

显示如何插入带有编号的新列表。

展示如何为周会准备模板。

显示如何将超链接绑定到文本。

### 也可以看看

* class [RichText](../../richtext)
* 命名空间 [Aspose.Note](../../richtext)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
