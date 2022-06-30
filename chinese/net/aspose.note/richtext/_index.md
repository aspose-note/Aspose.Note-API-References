---
title: RichText
second_title: Aspose.Note for .NET API 参考
description: 表示富文本
type: docs
weight: 510
url: /zh/net/aspose.note/richtext/
---
## RichText class

表示富文本。

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [RichText](richtext#constructor)() | 初始化[`RichText`](../richtext)类的新实例。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment) { get; set; } | 获取或设置对齐方式。 |
| [Document](../../aspose.note/node/document) { get; } | 获取节点的文档。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | 获取一个值，该值指示此节点是否为复合节点。如果为 true，则该节点可以有子节点。 |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime) { get; set; } | 获取或设置最后修改时间。 |
| [Length](../../aspose.note/richtext/length) { get; } | 获取文本的长度。 |
| [LineSpacing](../../aspose.note/richtext/linespacing) { get; set; } | 获取或设置行距。 |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype) { get; } | 获取节点类型。 |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle) { get; set; } | 获取或设置段落样式。 如果在Styles集合中没有匹配的 TextStyle 对象，或者此对象未指定所需的设置，则使用这些设置。 |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | 获取同一节点树级别的上一个节点。 |
| [SpaceAfter](../../aspose.note/richtext/spaceafter) { get; set; } | 获取或设置之后的最小空间量。 |
| [SpaceBefore](../../aspose.note/richtext/spacebefore) { get; set; } | 获取或设置之前的最小空间量。 |
| [Tags](../../aspose.note/richtext/tags) { get; } | 获取段落所有标签的列表。 |
| [Text](../../aspose.note/richtext/text) { get; set; } | 获取或设置文本。字符串不得包含任何值为 10 的字符（换行）。 |
| [TextRuns](../../aspose.note/richtext/textruns) { get; } | 获取文本运行的集合。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept)(DocumentVisitor) | 接受节点的访问者。 |
| [Append](../../aspose.note/richtext/append#append)(string) | 将字符串添加到最后一个文本范围。 |
| [Append](../../aspose.note/richtext/append#append_1)(string, TextStyle) | 在末尾添加一个字符串。 |
| [AppendFront](../../aspose.note/richtext/appendfront#appendfront)(string) | 将字符串添加到第一个文本范围的前面。 |
| [AppendFront](../../aspose.note/richtext/appendfront#appendfront_1)(string, TextStyle) | 在前面添加一个字符串。 |
| [Clear](../../aspose.note/richtext/clear)() | 清除此实例的内容。 |
| [GetEnumerator](../../aspose.note/richtext/getenumerator)() | 返回一个遍历此 RichText 对象的字符的枚举器。 |
| [IndexOf](../../aspose.note/richtext/indexof#indexof)(char) | 返回此字符串中指定 Unicode 字符第一次出现的从零开始的索引。 |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_3)(string) | 返回此实例中指定字符串第一次出现的从零开始的索引。 |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_1)(char, int) | 返回此字符串中指定 Unicode 字符第一次出现的从零开始的索引。搜索从指定的字符位置开始。 |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_4)(string, int) | 返回此实例中指定字符串第一次出现的从零开始的索引。搜索从指定的字符位置开始。 |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_8)(string, StringComparison) | 返回当前实例中指定字符串第一次出现的从零开始的索引。参数指定用于指定字符串的搜索类型。 |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_2)(char, int, int) | 返回此实例中指定字符第一次出现的从零开始的索引。搜索从指定的字符位置开始并检查指定数量的字符位置。 |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_5)(string, int, int) | 返回此实例中指定字符串第一次出现的从零开始的索引。搜索从指定的字符位置开始并检查指定数量的字符位置。 |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_7)(string, int, StringComparison) | 返回当前实例中指定字符串第一次出现的从零开始的索引。参数指定当前字符串中的起始搜索位置以及用于指定字符串的搜索类型。 |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_6)(string, int, int, StringComparison) | 返回当前实例中指定字符串第一次出现的从零开始的索引。 |
| [Insert](../../aspose.note/richtext/insert#insert)(int, string) | 在此实例中的指定索引位置插入指定字符串。 |
| [Insert](../../aspose.note/richtext/insert#insert_1)(int, string, TextStyle) | 在此实例中的指定索引位置插入具有指定样式的指定字符串。 |
| [Remove](../../aspose.note/richtext/remove#remove)(int) | 删除当前实例中的所有字符，从指定位置开始一直到最后一个位置。 |
| [Remove](../../aspose.note/richtext/remove#remove_1)(int, int) | 删除当前实例中从指定位置开始的指定数量的字符。 |
| [Replace](../../aspose.note/richtext/replace#replace)(char, char) | 将此实例中所有出现的指定 Unicode 字符替换为另一个指定的 Unicode 字符。 |
| [Replace](../../aspose.note/richtext/replace#replace_1)(string, string) | 将当前实例中出现的所有指定字符串替换为另一个指定字符串。 |
| [Replace](../../aspose.note/richtext/replace#replace_2)(string, string, TextStyle) | 用指定样式的另一个指定字符串替换当前实例中所有出现的指定字符串。 |
| [Trim](../../aspose.note/richtext/trim#trim)() | 删除所有前导和尾随空白字符。 |
| [Trim](../../aspose.note/richtext/trim#trim_1)(char) | 删除字符的所有前导和尾随实例。 |
| [Trim](../../aspose.note/richtext/trim#trim_2)(params char[]) | 删除数组中指定的一组字符的所有前导和尾随出现。 |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend)() | 删除所有尾随空白字符。 |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend_1)(char) | 删除所有尾随出现的字符。 |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend_2)(params char[]) | 删除数组中指定的一组字符的所有尾随出现。 |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart)() | 删除所有前导空白字符。 |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart_1)(char) | 删除指定字符的所有前导匹配项。 |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart_2)(params char[]) | 删除数组中指定的一组字符的所有前导匹配项。 |

### 例子

显示如何从文档中获取所有文本。

```csharp
// 加载 OneNote 文档
string dataDir = RunExamples.GetDataDir_Text();

// 克隆到没有历史记录的新文档
Document oneFile = new Document(dataDir + "Aspose.one");

// 克隆到具有历史记录的新文档
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// 文档目录的路径。
Console.WriteLine(text);
```

```csharp
// 加载 OneNote 文档并获取第一个孩子
string dataDir = RunExamples.GetDataDir_Text();

// 阅读本页的内容修订摘要
Document oneFile = new Document(dataDir + "Aspose.one");

// 更新此页面的页面修订摘要
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // 加载 OneNote 文档
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // 默认情况下，冲突页面只是在保存时跳过。
    Console.WriteLine(text);
}
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 如果将其标记为非冲突，那么它将像往常一样保存在历史记录中。
Document document = new Document(dataDir + "Aspose.one");

// 文档目录的路径。
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
// 加载 OneNote 文档并获取第一个孩子
string dataDir = RunExamples.GetDataDir_Tables();

// 阅读本页的内容修订摘要
Document document = new Document(dataDir + "Sample1.one");

// 更新此页面的页面修订摘要
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // 加载 OneNote 文档
    foreach (TableRow row in table)
    {
        // 默认情况下，冲突页面只是在保存时跳过。
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // 如果将其标记为非冲突，那么它将像往常一样保存在历史记录中。
        Console.WriteLine(text);
    }
}
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tables();

// 加载 OneNote 文档并获取第一个孩子
Document document = new Document(dataDir + "Sample1.one");

// 阅读本页的内容修订摘要
IList<Table> nodes = document.GetChildNodes<Table>();

// 更新此页面的页面修订摘要
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // 加载 OneNote 文档
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // 默认情况下，冲突页面只是在保存时跳过。
    Console.WriteLine(text);
}
```

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 如果将其标记为非冲突，那么它将像往常一样保存在历史记录中。
Document document = new Document(dataDir + "Aspose.one");

// 文档目录的路径。
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // 将文档加载到 Aspose.Note。
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // 将文档加载到 Aspose.Note。
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
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

```csharp
// 在输出屏幕上打印文本
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Aspose.one");

// 将文档加载到 Aspose.Note。
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 获取页面节点列表
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// 获取文本
oneFile.Save(dataDir, SaveFormat.Pdf);
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
// 遍历表行
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note。
Document document = new Document(dataDir + "Sample1.one");

// 遍历页面的标题。
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    的头衔。
    foreach (TableRow row in table)
    {
        // 文档目录的路径。
        // 将文档加载到 Aspose.Note。
        foreach (TableCell cell in row)
        {
            // 获取表节点列表
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // 遍历表行
            Console.WriteLine(text);
        }
    }
}
```

```csharp
// 获取文本
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// 在输出屏幕上打印文本
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// 文档目录的路径。
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 将文档加载到 Aspose.Note。
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// 获取表节点列表
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

```csharp
// 设置表数
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 获取文本
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// 在输出屏幕上打印文本
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// 将文档加载到 Aspose.Note。
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

```csharp
// 获取上周修改的 RichText 节点。
string dataDir = RunExamples.GetDataDir_Tags();

// 设置高亮颜色
Document doc = new Document();

// 设置高亮颜色
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 文档目录的路径。
Outline outline = new Outline(doc);

// 将文档加载到 Aspose.Note。
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// 获取所有富文本节点
outlineElem.AppendChildLast(text);

// 替换形状的文本
outline.AppendChildLast(outlineElem);

// 保存为任何支持的文件格式
page.AppendChildLast(outline);

// 文档目录的路径。
doc.AppendChildLast(page);

// 将文档加载到 Aspose.Note。
dataDir = dataDir + "AddTextNodeWithTag_out.one";
doc.Save(dataDir);
```

```csharp
// 获取表节点列表
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 遍历表行
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// 获取 TableCell 节点列表
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 遍历表格单元格
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

```csharp
// 获取文本
string dataDir = RunExamples.GetDataDir_Tags();

// 在输出屏幕上打印文本
Document oneFile = new Document(dataDir + "TagFile.one");

// 文档目录的路径。
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// 将文档加载到 Aspose.Note。
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // 获取所有富文本节点
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
// 替换形状的文本
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 保存为任何支持的文件格式
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

让我们通过增加字体大小在其他标题中强调页面标题。

显示如何从每个表的行中获取文本。

显示如何从表中获取文本。

让我们通过突出显示来强调最新文本的更改。

显示如何为页面设置标题。

设置文本的校对语言。

显示如何通过所有页面并在文本中进行替换。

使用段落样式按文本格式进行操作。

显示如何从表格的单元格中获取文本。

显示如何通过页面文本并进行替换。

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

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [ITaggable](../itaggable)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
