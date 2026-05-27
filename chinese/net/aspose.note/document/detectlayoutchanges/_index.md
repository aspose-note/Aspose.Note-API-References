---
title: "Document.DetectLayoutChanges"
second_title: "Aspose.Note for .NET API 参考"
description: "Document 方法。检测自上一次 DetectLayoutChanges 调用以来对文档布局所做的所有更改。如果 AutomaticLayoutChangesDetectionEnabled 设置为 true，则在文档导出开始时自动使用。"
type: docs
weight: 90
url: /zh/net/aspose.note/document/detectlayoutchanges/
---
## Document.DetectLayoutChanges method

检测自上一次 `DetectLayoutChanges` 调用以来对文档布局所做的所有更改。如果 [`AutomaticLayoutChangesDetectionEnabled`](../automaticlayoutchangesdetectionenabled/) 设置为 true，则在文档导出开始时自动使用。

```csharp
public void DetectLayoutChanges()
```

## 示例

展示如何将文档保存为不同的格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化新的 Document
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 初始化新页面
Page page = new Page();

// 文档中所有文本的默认样式。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// 追加页面节点
doc.AppendChildLast(page);

// 以不同格式保存 OneNote 文档，设置文本字体大小并手动检测布局更改。
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


