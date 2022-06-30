---
title: NumberList
second_title: Aspose.Note for .NET API 参考
description: 获取或设置编号列表标题的样式
type: docs
weight: 50
url: /zh/net/aspose.note/outlineelement/numberlist/
---
## OutlineElement.NumberList property

获取或设置编号列表标题的样式。

```csharp
public NumberList NumberList { get; set; }
```

### 例子

显示如何检索有关列表格式的信息。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

//------------------------
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

//------------------------
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

//------------------------
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // 保存 OneNote 文档
        Console.WriteLine("Font Name: " + list.Font);

        // 创建 Document 类的对象
        Console.WriteLine("Font Length: " + list.Font.Length);

        //初始化Page类对象
        Console.WriteLine("Font Size: " + list.FontSize);

        // 初始化大纲类对象
        Console.WriteLine("Font Color: " + list.FontColor);

        // 初始化 TextStyle 类对象并设置格式属性
        Console.WriteLine("Font format: " + list.Format);

        // 初始化 OutlineElement 类对象并应用项目符号
        Console.WriteLine("Is bold: " + list.IsBold);

        // 初始化 RichText 类对象并应用文本样式
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 添加轮廓元素
Aspose.Note.Document doc = new Aspose.Note.Document();

// 添加大纲节点
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// 添加页面节点
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 TextStyle 类对象并设置格式属性
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

// 创建 Document 类的对象
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

// 创建 Document 类的对象
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 创建 Document 类的对象
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// 初始化 TextStyle 类对象并设置格式属性
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 初始化 OutlineElement 类对象并应用编号
Aspose.Note.Document doc = new Aspose.Note.Document();

// 同一大纲中的数字会自动递增。
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 将文档加载到 Aspose.Note。
Outline outline = new Outline(doc);

// 获取大纲元素的集合节点
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 遍历每个节点
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// 获取字体名称
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 将文档加载到 Aspose.Note。
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 获取大纲元素的集合节点
page.AppendChildLast(outline);
// 遍历每个节点
doc.AppendChildLast(page);

// 获取字体名称
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 获取字体长度
Document doc = new Document();

// 获取字体大小
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 获取字体颜色
Outline outline = new Outline(doc);

// 获取格式
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 检查粗体
// 检查斜体
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 初始化 OneNote 文档
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 初始化 OneNote 页面
page.AppendChildLast(outline);

// 应用文本样式设置
doc.AppendChildLast(page);

// 同一大纲中的数字会自动递增。
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

显示如何插入带有中文编号的新列表。

显示如何插入新的项目符号列表。

显示如何插入带有编号的新列表。

### 也可以看看

* class [NumberList](../../numberlist)
* class [OutlineElement](../../outlineelement)
* 命名空间 [Aspose.Note](../../outlineelement)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
