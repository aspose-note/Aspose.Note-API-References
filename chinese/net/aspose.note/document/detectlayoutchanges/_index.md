---
title: Document.DetectLayoutChanges
second_title: Aspose.Note for .NET API 参考
description: Document 方法. 检测自上次以来对文档布局所做的所有更改DetectLayoutChangescall. 万一AutomaticLayoutChangesDetectionEnabled设置为 true在文档导出开始时自动使用
type: docs
weight: 90
url: /zh/net/aspose.note/document/detectlayoutchanges/
---
## Document.DetectLayoutChanges method

检测自上次以来对文档布局所做的所有更改`DetectLayoutChanges`call. 万一[`AutomaticLayoutChangesDetectionEnabled`](../automaticlayoutchangesdetectionenabled/)设置为 true，在文档导出开始时自动使用。

```csharp
public void DetectLayoutChanges()
```

### 例子

显示如何以不同格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 初始化新文档
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// 初始化新页面
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// 文档中所有文本的默认样式。
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

//追加页面节点
doc.AppendChildLast(page);

// 以不同格式保存 OneNote 文档，手动设置文本字体大小和检测布局变化。
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### 也可以看看

* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)


