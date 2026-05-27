---
title: "RunIndex"
second_title: "Aspose.Note for .NET API 参考"
description: 
type: docs
weight: 100
url: /zh/net/aspose.note/textstyle/runindex/
---
## TextStyle.RunIndex property

获取或设置运行索引。

```csharp
public int RunIndex { get; set; }
```

### 备注

运行索引指定将在文本节点中使用此样式的最后一个符号的编号。第一个符号被定义为紧随前一个样式在样式集合中最后一个符号之后。索引从 1 开始。

### 示例

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
* namespace [Aspose.Note](../../textstyle)
* assembly [Aspose.Note](../../../)

<!-- 请勿编辑：由 xmldocmd 为 Aspose.Note.dll 生成 -->
