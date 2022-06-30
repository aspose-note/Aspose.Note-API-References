---
title: Title
second_title: Aspose.Note for .NET API 参考
description: 获取或设置标题
type: docs
weight: 120
url: /zh/net/aspose.note/page/title/
---
## Page.Title property

获取或设置标题。

```csharp
public Title Title { get; set; }
```

### 适当的价值

`Title`。

### 例子

显示如何获取有关页面的元信息。

```csharp
// 保存 OneNote 文档
string dataDir = RunExamples.GetDataDir_Pages();

// 创建 Document 类的对象
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

```csharp
//初始化Page类对象
string dataDir = RunExamples.GetDataDir_Pages();

// 初始化大纲类对象           
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
// 初始化 TextStyle 类对象并设置格式属性
string dataDir = RunExamples.GetDataDir_Pages();

// 初始化 OutlineElement 类对象并应用编号
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 同一大纲中的数字会自动递增。
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

```csharp
// 添加轮廓元素
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 添加大纲节点
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// 添加页面节点
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// 保存 OneNote 文档
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 创建 Document 类的对象
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 初始化 Page 类对象并设置它的层级
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 初始化 Page 类对象并设置它的层级
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

```csharp
// 初始化 Page 类对象并设置它的层级
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 加载 OneNote 文档
Document doc = new Aspose.Note.Document();

// 文档目录的路径。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 加载 OneNote 文档并获取第一个孩子
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 阅读本页的内容修订摘要
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 更新此页面的页面修订摘要
doc.AppendChildLast(page);

// 加载 OneNote 文档
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

```csharp
// 默认情况下，冲突页面只是在保存时跳过。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 如果将其标记为非冲突，那么它将像往常一样保存在历史记录中。
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 文档目录的路径。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 将文档加载到 Aspose.Note。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// 文档目录的路径。
doc.AppendChildLast(page);

// 加载 OneNote 文档并获取第一个孩子
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

显示如何编辑页面的历史记录。

显示如何为页面设置标题。

显示如何获取页面的历史记录。

显示如何使用默认选项创建文档并将其保存为 html 格式。

显示如何创建文档并以 html 格式保存指定范围的页面。

显示如何创建带有标题页的文档。

显示如何以不同格式保存文档。

### 也可以看看

* class [Title](../../title)
* class [Page](../../page)
* 命名空间 [Aspose.Note](../../page)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
