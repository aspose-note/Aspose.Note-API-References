---
title: TextStyle.HyperlinkAddress
second_title: Aspose.Note for .NET API 参考
description: TextStyle 财产. 获取或设置超链接地址必须设置如果值IsHyperlink属性为真
type: docs
weight: 60
url: /zh/net/aspose.note/textstyle/hyperlinkaddress/
---
## TextStyle.HyperlinkAddress property

获取或设置超链接地址。必须设置，如果值[`IsHyperlink`](../ishyperlink/)属性为真。

```csharp
public string HyperlinkAddress { get; set; }
```

### 例子

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

* class [TextStyle](../)
* 命名空间 [Aspose.Note](../../textstyle/)
* 部件 [Aspose.Note](../../../)


