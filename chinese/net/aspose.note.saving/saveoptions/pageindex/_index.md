---
title: PageIndex
second_title: Aspose.Note for .NET API 参考
description: 获取或设置要保存的第一页的索引默认为 0
type: docs
weight: 30
url: /zh/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

获取或设置要保存的第一页的索引。默认为 0。

```csharp
public int PageIndex { get; set; }
```

### 例子

显示如何以 png 格式保存文档。

```csharp
// 初始化 PdfSaveOptions 对象
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 使用 Jpeg 压缩
Document oneFile = new Document(dataDir + "Aspose.one");

// JPEG 压缩的质量 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // 文档目录的路径。
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// 加载 OneNote 笔记本
oneFile.Save(dataDir, opts);
```

```csharp
// 保存笔记本
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
Document oneFile = new Document(dataDir + "Aspose.one");

// 将文档加载到 Aspose.Note。
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 或者
                              PageIndex = 0,

                              // 文档目录的路径。
                              PageCount = 1,
                          };

// 将文档加载到 Aspose.Note。
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

```csharp
// 或者
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 或者
Document doc = new Document(dataDir + "Aspose.one");

// 或者
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 或者
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // 文档目录的路径。
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 文档目录的路径。
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

// 文档目录的路径。
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

// 将文档加载到 Aspose.Note。
Document doc = new Document();

// 将文档保存为 PDF
Page page = new Page();

// 文档目录的路径。
Title title = new Title();

// 将文档加载到 Aspose.Note。
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

// 将文档保存为 PDF
page.Title = title;

// 文档目录的路径。
outlineElem.AppendChildLast(text);

// 将文档加载到 Aspose.Note。
outline.AppendChildLast(outlineElem);

// 将文档保存为 PDF
page.AppendChildLast(outline);

// 文档目录的路径。
doc.AppendChildLast(page);

// 将文档加载到 Aspose.Note。
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

显示如何以 pdf 格式保存文档。

显示如何使用特定设置以 pdf 格式保存文档。

显示如何创建文档并以 html 格式保存指定范围的页面。

展示如何使用格式化的富文本创建文档。

### 也可以看看

* class [SaveOptions](../../saveoptions)
* 命名空间 [Aspose.Note.Saving](../../saveoptions)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
