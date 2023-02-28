---
title: ImageSaveOptions.Resolution
second_title: Aspose.Note for .NET API 参考
description: ImageSaveOptions 财产. 获取或设置生成图像的分辨率以每英寸点数为单位
type: docs
weight: 50
url: /zh/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

获取或设置生成图像的分辨率，以每英寸点数为单位。

```csharp
public float Resolution { get; set; }
```

### 评论

默认值为 96.

### 例子

显示将文档另存为图像时如何设置图像分辨率。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// 保存文档。
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

显示如何使用指定选项将笔记本另存为图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载一个 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

展示如何将扁平笔记本另存为图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载一个 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

### 也可以看看

* class [ImageSaveOptions](../)
* 命名空间 [Aspose.Note.Saving](../../imagesaveoptions/)
* 部件 [Aspose.Note](../../../)


