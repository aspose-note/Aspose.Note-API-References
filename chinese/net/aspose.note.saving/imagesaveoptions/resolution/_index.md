---
title: "ImageSaveOptions.Resolution"
second_title: "Aspose.Note for .NET API 参考"
description: "ImageSaveOptions 属性。获取或设置生成图像的分辨率（每英寸点数）"
type: docs
weight: 50
url: /zh/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

获取或设置生成图像的分辨率（每英寸点数）。

```csharp
public float Resolution { get; set; }
```

## 备注

默认值为 96。

## 示例

展示如何在将文档保存为图像时设置图像分辨率。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 保存文档。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

展示如何使用指定选项将笔记本保存为图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

展示如何将扁平化的笔记本保存为图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

### 另请参阅

* class [ImageSaveOptions](../)
* namespace [Aspose.Note.Saving](../../imagesaveoptions/)
* assembly [Aspose.Note](../../../)


