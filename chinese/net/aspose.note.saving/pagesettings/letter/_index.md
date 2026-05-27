---
title: "PageSettings.Letter"
second_title: "Aspose.Note for .NET API 参考"
description: "PageSettings 属性。获取 Letter 格式页面的设置"
type: docs
weight: 30
url: /zh/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

获取 Letter 格式页面的设置。

```csharp
public static PageSettings Letter { get; }
```

## 示例

展示如何将文档保存为 Pdf 格式并使用 Letter 页面布局。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// 保存文档。
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

### 另请参阅

* class [PageSettings](../)
* namespace [Aspose.Note.Saving](../../pagesettings/)
* assembly [Aspose.Note](../../../)


