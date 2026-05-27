---
title: "Styles"
second_title: "Aspose.Note for .NET API 参考"
description: 
type: docs
weight: 80
url: /zh/net/aspose.note/richtext/styles/
---
## RichText.Styles property

获取样式。

```csharp
public IList<TextStyle> Styles { get; }
```

### 示例

展示如何更改文本的样式。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "Aspose.one");

// 获取特定的 RichText 节点
RichText richText = document.GetChildNodes<RichText>().First();

foreach (TextStyle style in richText.Styles)
{
    // 设置字体颜色
    style.FontColor = Color.Yellow;

    // 设置高亮颜色
    style.Highlight = Color.Blue;

    // 设置字体大小
    style.FontSize = 20;
}
```

让我们格式化表格以获得更好的可读性。将标题行设为粗体和斜体，使用 LightGray 颜色突出显示每个偶数行。

```csharp
string dataDir = RunExamples.GetDataDir_Tables();

// 将文档加载到 Aspose.Note 中。
Document document = new Document(dataDir + "ChangeTableStyleIn.one");

// 获取表格节点列表
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    SetRowStyle(table.First(), Color.DarkGray, true, true);

    // 突出显示标题后的第一行。
    var flag = false;
    foreach (var row in table.Skip(1))
    {
        SetRowStyle(row, flag ? Color.LightGray : Color.Empty, false, false);

        flag = !flag;
    }
}

document.Save(Path.Combine(dataDir, "ChangeTableStyleOut.one"));
```

为文本设置校对语言。

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { Text = "United States Germany China", ParagraphStyle = ParagraphStyle.Default };
text.Styles.Add(new TextStyle()
                    {
                        Language = CultureInfo.GetCultureInfo("en-US"),
                        RunIndex = 13
                    });
text.Styles.Add(new TextStyle()
                    {
                        Language = CultureInfo.GetCultureInfo("de-DE"),
                        RunIndex = 21
                    });
text.Styles.Add(new TextStyle()
                    {
                        Language = CultureInfo.GetCultureInfo("zh-CN"),
                        RunIndex = text.Text.Length
                    });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
```

展示如何将超链接绑定到文本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Tasks();

// 创建 Document 类的对象
Document doc = new Document();

RichText titleText = new RichText()
                     {
                         Text = "Title!",
                         ParagraphStyle = ParagraphStyle.Default
                     };

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

                             // 此样式将应用于 0-7 个字符。
                             RunIndex = 8 
                         };

TextStyle textStyleHyperlink = new TextStyle
                              {
                                  // 此样式将应用于 8-16 个字符。
                                  RunIndex = 17,
                                  HyperlinkAddress = "https://www.google.com"
                              };

RichText text = new RichText()
                {
                    Text = "This is hyperlink. This text is not a hyperlink.",
                    ParagraphStyle = ParagraphStyle.Default,
                    Styles = { textStyleRed, textStyleHyperlink }
                };

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// 添加大纲元素
outline.AppendChildLast(outlineElem);

// 初始化 Title 类对象
Title title = new Title() { TitleText = titleText };

// 初始化 Page 类对象
Aspose.Note.Page page = new Aspose.Note.Page(doc) { Title = title };

// 添加 Outline 节点
page.AppendChildLast(outline);

// 添加 Page 节点
doc.AppendChildLast(page);

// 保存 OneNote 文档
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

### 另请参阅

* class [TextStyle](../../textstyle)
* class [RichText](../../richtext)
* namespace [Aspose.Note](../../richtext)
* assembly [Aspose.Note](../../../)

<!-- 请勿编辑：由 xmldocmd 为 Aspose.Note.dll 生成 -->
