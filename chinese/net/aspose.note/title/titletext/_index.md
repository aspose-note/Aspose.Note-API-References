---
title: TitleText
second_title: Aspose.Note for .NET API 参考
description: 获取或设置标题的文本
type: docs
weight: 60
url: /zh/net/aspose.note/title/titletext/
---
## Title.TitleText property

获取或设置标题的文本。

```csharp
public RichText TitleText { get; set; }
```

### 例子

显示如何编辑页面的历史记录。

```csharp
// 初始化大纲对象
string dataDir = RunExamples.GetDataDir_Pages();

// 初始化 OutlineElement 对象           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
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
// 将表格添加到大纲元素节点
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 添加大纲元素到大纲
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// 添加大纲到页面节点
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// 添加页面到文档节点
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 加载 OneNote 文档并获取第一个孩子
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 文档目录的路径。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 初始化 OneNote 文档
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

```csharp
// 初始化 OneNote 文档
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 保存为 HTML 格式
Document doc = new Aspose.Note.Document();

// 文档目录的路径。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 初始化 OneNote 文档
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 文档中所有文本的默认样式。
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 保存为 HTML 格式
doc.AppendChildLast(page);

// 文档目录的路径。
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

```csharp
// 创建 Document 类的对象
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

//初始化Page类对象
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 设置页面标题属性
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 设置页面标题属性
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 在文档中追加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

显示如何为页面设置标题。

显示如何使用默认选项创建文档并将其保存为 html 格式。

显示如何创建文档并以 html 格式保存指定范围的页面。

显示如何创建带有标题页的文档。

显示如何以不同格式保存文档。

### 也可以看看

* class [RichText](../../richtext)
* class [Title](../../title)
* 命名空间 [Aspose.Note](../../title)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
