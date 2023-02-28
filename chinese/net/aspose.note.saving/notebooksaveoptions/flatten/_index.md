---
title: NotebookSaveOptions.Flatten
second_title: Aspose.Note for .NET API 参考
description: NotebookSaveOptions 财产. 获取或设置一个值该值指示笔记本子层次结构是否以扁平化方式保存
type: docs
weight: 20
url: /zh/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

获取或设置一个值，该值指示笔记本子层次结构是否以扁平化方式保存。

```csharp
public bool Flatten { get; set; }
```

### 例子

展示如何以 pdf 格式保存扁平笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载一个 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// 保存笔记本
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
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

* class [NotebookSaveOptions](../)
* 命名空间 [Aspose.Note.Saving](../../notebooksaveoptions/)
* 部件 [Aspose.Note](../../../)


