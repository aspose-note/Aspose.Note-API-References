---
title: "类 RichText"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.RichText 类。表示富文本。"
type: docs
weight: 610
url: /zh/net/aspose.note/richtext/
---
## RichText class

表示富文本。

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RichText](richtext/)() | 初始化 `RichText` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | 获取或设置对齐方式。 |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | 获取一个值，指示此节点是否为复合节点。如果为 true，则该节点可以拥有子节点。 |
| [IsTitleDate](../../aspose.note/richtext/istitledate/) { get; } | 获取一个值，指示 RichText 元素是否在页面标题中包含日期。 |
| [IsTitleText](../../aspose.note/richtext/istitletext/) { get; } | 获取一个值，指示 RichText 元素是否在页面标题中包含文本。 |
| [IsTitleTime](../../aspose.note/richtext/istitletime/) { get; } | 获取一个值，指示 RichText 元素是否在页面标题中包含时间。 |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | 获取或设置最后修改时间。 |
| [Length](../../aspose.note/richtext/length/) { get; } | 获取文本的长度。 |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | 获取或设置行间距。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树层级的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | 获取或设置段落样式。如果在 Styles 集合中没有匹配的 TextStyle 对象，或者此对象未指定所需设置，则使用这些设置。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树层级的上一个节点。 |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | 获取或设置之后的最小间距。 |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | 获取或设置之前的最小间距。 |
| [Tags](../../aspose.note/richtext/tags/) { get; } | 获取段落的所有标签列表。 |
| [Text](../../aspose.note/richtext/text/) { get; set; } | 获取或设置文本。字符串不得包含值为 10（换行）的任何字符。 |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | 获取文本运行的集合。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | 接受节点的访问者。 |
| [Append](../../aspose.note/richtext/append/#append)(string) | 向最后的文本范围添加字符串。 |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | 在末尾添加字符串。 |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | 在第一个文本范围的前面添加字符串。 |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | 在前面添加字符串。 |
| [Clear](../../aspose.note/richtext/clear/)() | 清除此实例的内容。 |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | 返回一个枚举器，用于遍历此 RichText 对象的字符。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | 返回此字符串中指定 Unicode 字符首次出现的零基索引。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | 返回此实例中指定字符串首次出现的零基索引。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | 返回此字符串中指定 Unicode 字符首次出现的零基索引。搜索从指定的字符位置开始。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | 返回此实例中指定字符串首次出现的零基索引。搜索从指定的字符位置开始。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | 返回当前实例中指定字符串首次出现的零基索引。参数指定用于指定字符串的搜索类型。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | 返回此实例中指定字符首次出现的零基索引。搜索从指定的字符位置开始，并检查指定数量的字符位置。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | 返回此实例中指定字符串首次出现的零基索引。搜索从指定的字符位置开始，并检查指定数量的字符位置。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | 返回当前实例中指定字符串首次出现的零基索引。参数指定当前字符串的起始搜索位置以及用于指定字符串的搜索类型。 |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | 返回当前实例中指定字符串首次出现的零基索引。 |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | 在此实例的指定索引位置插入指定的字符串。 |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | 在此实例的指定索引位置插入具有指定样式的指定字符串。 |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | 从指定位置开始一直到最后位置，删除当前实例中的所有字符。 |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | 从指定位置开始，删除当前实例中指定数量的字符。 |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | 将此实例中所有指定的 Unicode 字符替换为另一个指定的 Unicode 字符。 |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | 将当前实例中所有指定的字符串替换为另一个指定的字符串。 |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | 将当前实例中所有指定的字符串替换为具有指定样式的另一个指定字符串。 |
| [Trim](../../aspose.note/richtext/trim/#trim)() | 删除所有前导和尾随的空白字符。 |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | 删除所有前导和尾随的字符实例。 |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | 删除数组中指定的一组字符的所有前导和尾随出现。 |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | 删除所有尾随的空白字符。 |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | 删除所有尾随的字符出现。 |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | 删除数组中指定的一组字符的所有尾随出现。 |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | 删除所有前导的空白字符。 |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | 删除所有指定字符的前导出现。 |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | 删除数组中指定的一组字符的所有前导出现。 |

## 示例

展示如何获取文档中的所有文本。

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

展示如何获取页面中的所有文本。

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

让我们通过增大字体大小来强调页面的标题，而不是其他标题。

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

展示如何从每个表格的行中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Sample1.one");

// 获取表格节点列表
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // 遍历表格行
    foreach (TableRow row in table)
    {
        // 检索文本
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // 在输出屏幕上打印文本
        Console.WriteLine(text);
    }
}
```

展示如何从表格中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Sample1.one");

// 获取表格节点列表
IList<Table> nodes = document.GetChildNodes<Table>();

// 设置表格计数
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

让我们通过高亮来强调最新文本的更改。

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

展示如何为页面设置标题。

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page();

page.Title = new Title()
{
    TitleText = new RichText()
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText()
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText()
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

为文本设置校对语言。

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

展示如何遍历所有页面并在文本中进行替换。

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

// 保存为任何受支持的文件格式
oneFile.Save(dataDir, SaveFormat.Pdf);
```

使用段落样式操作文本格式。

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

展示如何从表格的单元格中获取文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Sample1.one");

// 获取表格节点列表
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // 遍历表格行
    foreach (TableRow row in table)
    {
        // 获取 TableCell 节点列表
        // 遍历表格单元格
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

展示如何遍历页面的文本并进行替换。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// 获取所有 RichText 节点
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 替换形状的文本
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// 保存为任何受支持的文件格式
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

展示如何创建文档并使用默认选项将其保存为 HTML 格式。

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

// 保存为 HTML 格式
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

展示如何添加带标签的新段落。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象
Outline outline = new Outline();

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement();
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText() { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// 添加文本节点
outlineElem.AppendChildLast(text);

// 添加大纲元素节点
outline.AppendChildLast(outlineElem);

// 添加大纲节点
page.AppendChildLast(outline);

// 添加页面节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

展示如何创建文档并在指定页面范围内以 HTML 格式保存。

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

// 保存为 HTML 格式
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

展示如何访问标签的详细信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "TagFile.one");

// 获取所有 RichText 节点
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 遍历每个节点
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

展示如何使用文本创建文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象
Outline outline = new Outline();

// 初始化 OutlineElement 类对象
OutlineElement outlineElem = new OutlineElement();

// 初始化 TextStyle 类对象并设置格式属性
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 RichText 类对象并应用文本样式
RichText text = new RichText() { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// 添加 RichText 节点
outlineElem.AppendChildLast(text);

// 添加 OutlineElement 节点
outline.AppendChildLast(outlineElem);

// 添加 Outline 节点
page.AppendChildLast(outline);

// 添加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

展示如何插入带中文编号的新列表。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 初始化 OneNote 文档
Document doc = new Document();

// 初始化 OneNote 页面
Page page = new Page();
Outline outline = new Outline();

// 应用文本样式设置
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 同一大纲中的数字会自动递增。
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
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

展示如何插入新的项目符号列表。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象
Outline outline = new Outline();

// 初始化 TextStyle 类对象并设置格式属性
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 OutlineElement 类对象并应用项目符号
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };

// 初始化 RichText 类对象并应用文本样式
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(  ) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 添加大纲元素
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 添加 Outline 节点
page.AppendChildLast(outline);
// 添加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

展示如何插入带编号的新列表。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 创建 Document 类的对象
Document doc = new Document();

// 初始化 Page 类对象
Page page = new Page();

// 初始化 Outline 类对象
Outline outline = new Outline();

// 初始化 TextStyle 类对象并设置格式属性
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// 初始化 OutlineElement 类对象并应用编号
// 同一大纲中的数字会自动递增。
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// 添加大纲元素
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// 添加 Outline 节点
page.AppendChildLast(outline);

// 添加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

展示如何准备每周会议的模板。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tags();

// 创建 Document 类的对象
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

展示如何将超链接绑定到文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tasks();

// 创建 Document 类的对象
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
                                       HyperlinkAddress = "https://www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// 添加大纲元素
outline.AppendChildLast(outlineElem);

// 初始化 Title 类对象
Title title = new Title() { TitleText = titleText };

// 初始化 Page 类对象
Page page = new Note.Page() { Title = title };

// 添加 Outline 节点
page.AppendChildLast(outline);

// 添加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### 另请参阅

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


