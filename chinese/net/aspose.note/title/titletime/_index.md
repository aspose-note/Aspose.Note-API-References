---
title: TitleTime
second_title: Aspose.Note for .NET API 参考
description: 获取或设置标题中时间的字符串表示
type: docs
weight: 70
url: /zh/net/aspose.note/title/titletime/
---
## Title.TitleTime property

获取或设置标题中时间的字符串表示。

```csharp
public RichText TitleTime { get; set; }
```

### 例子

显示如何设置页面标题。

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
// 在文档中追加 Page 节点
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 保存 OneNote 文档
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

// 初始化新文档
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

```csharp
// 初始化新页面
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 追加页面节点
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 追加页面节点
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 以不同格式保存 OneNote 文档，设置文本字体大小并手动检测布局变化。
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化 OneNote 文档
Document doc = new Aspose.Note.Document();

// 保存为 HTML 格式
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 保存为 HTML 格式
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 文档目录的路径。
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 初始化 OneNote 文档
doc.AppendChildLast(page);

// 文档中所有文本的默认样式。
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

```csharp
// 保存为 HTML 格式
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 创建 Document 类的对象
Aspose.Note.Page page = new Aspose.Note.Page(doc);

//初始化Page类对象
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 文档中所有文本的默认样式。
doc.AppendChildLast(page);

// 设置页面标题属性
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

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
