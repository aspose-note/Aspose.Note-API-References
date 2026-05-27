---
title: "NotebookSaveOptions.Flatten"
second_title: "Aspose.Note for .NET API 参考"
description: "NotebookSaveOptions 属性。获取或设置一个值，指示是否以扁平化方式保存笔记本子层级结构"
type: docs
weight: 20
url: /zh/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

获取或设置一个值，指示是否将笔记本子层次结构保存为扁平化。

```csharp
public bool Flatten { get; set; }
```

## 示例

展示如何以 PDF 格式保存扁平化的笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

// 保存笔记本
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
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

* class [NotebookSaveOptions](../)
* namespace [Aspose.Note.Saving](../../notebooksaveoptions/)
* assembly [Aspose.Note](../../../)


