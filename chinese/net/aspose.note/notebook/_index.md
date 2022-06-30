---
title: Notebook
second_title: Aspose.Note for .NET API 参考
description: 代表一个 Aspose.Note 笔记本
type: docs
weight: 390
url: /zh/net/aspose.note/notebook/
---
## Notebook class

代表一个 Aspose.Note 笔记本。

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Notebook](notebook#constructor)() | 初始化[`Notebook`](../notebook)类的新实例。 |
| [Notebook](notebook#constructor_1)(Stream) | 初始化[`Notebook`](../notebook)类的新实例。 从流中打开现有的 OneNote 笔记本。 |
| [Notebook](notebook#constructor_3)(string) | 初始化[`Notebook`](../notebook)类的新实例。 从文件中打开现有的 OneNote 笔记本。 |
| [Notebook](notebook#constructor_2)(Stream, NotebookLoadOptions) | 初始化[`Notebook`](../notebook)类的新实例。 从流中打开现有的 OneNote 笔记本。允许指定其他加载选项。 |
| [Notebook](notebook#constructor_4)(string, NotebookLoadOptions) | 初始化[`Notebook`](../notebook)类的新实例。 从文件中打开现有的 OneNote 笔记本。允许指定其他选项，例如子加载策略（“懒惰”/即时）。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Color](../../aspose.note/notebook/color) { get; set; } | 获取或设置颜色。 |
| [Count](../../aspose.note/notebook/count) { get; } | 获取[`Notebook`](../notebook)中包含的元素数量。 |
| [DisplayName](../../aspose.note/notebook/displayname) { get; set; } | 获取或设置显示名称。 |
| [FileFormat](../../aspose.note/notebook/fileformat) { get; } | 获取文件格式（OneNote 2010、OneNote Online）。 |
| [Guid](../../aspose.note/notebook/guid) { get; } | 获取对象的全局唯一 ID。 |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled) { get; set; } | 获取或设置一个指示是否启用历史记录的值。 |
| [Item](../../aspose.note/notebook/item) { get; } | 通过给定索引获取笔记本子节点。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild)(INotebookChildNode) | 将节点添加到列表的末尾。 |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes)() | 按节点类型获取所有子节点。 |
| [GetEnumerator](../../aspose.note/notebook/getenumerator)() | 返回一个遍历[`Notebook`](../notebook)的子节点的枚举器。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument)(Stream) | 添加一个子文档节点。 从流中打开现有 OneNote 文档。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_2)(string) | 添加一个子文档节点。 从文件中打开现有的 OneNote 文档。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_1)(Stream, LoadOptions) | 添加一个子文档节点。 从流中打开现有 OneNote 文档。允许指定其他加载选项。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_3)(string, LoadOptions) | 添加一个子文档节点。 从文件中打开现有的 OneNote 文档。允许指定其他加载选项。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook)(Stream) | 添加一个子笔记本节点。 从流中打开现有的 OneNote 笔记本。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_2)(string) | 添加一个子笔记本节点。 从文件中打开现有的 OneNote 笔记本。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_1)(Stream, NotebookLoadOptions) | 添加一个子笔记本节点。 从流中打开现有的 OneNote 笔记本。允许指定其他加载选项。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_3)(string, NotebookLoadOptions) | 添加一个子笔记本节点。 从文件中打开现有的 OneNote 笔记本。允许指定其他加载选项。 |
| [RemoveChild](../../aspose.note/notebook/removechild)(INotebookChildNode) | 删除子节点。 |
| [Save](../../aspose.note/notebook/save#save)(Stream) | 将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/notebook/save#save_3)(string) | 将 OneNote 文档保存到文件中。 |
| [Save](../../aspose.note/notebook/save#save_2)(Stream, NotebookSaveOptions) | 使用指定的保存选项将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/notebook/save#save_1)(Stream, SaveFormat) | 将 OneNote 文档以指定格式保存到流中。 |
| [Save](../../aspose.note/notebook/save#save_5)(string, NotebookSaveOptions) | 使用指定的保存选项将 OneNote 文档保存到文件中。 |
| [Save](../../aspose.note/notebook/save#save_4)(string, SaveFormat) | 将 OneNote 文档保存到指定格式的文件中。 |

### 例子

显示如何保存笔记本。

```csharp
// 添加页面节点
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// 保存 OneNote 文档
notebook.Save(dataDir);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 文档目录的路径。
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// 文档目录的路径。
notebook.Save(dataDir);
```

```csharp
//image.com" };
string dataDir = RunExamples.GetDataDir_NoteBook();

// 实例化许可证类
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// 仅传递嵌入在程序集中的许可文件的名称
notebook.Save(dataDir);
```

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

```csharp
// 实例化许可证类
string dataDir = RunExamples.GetDataDir_NoteBook();

// 仅传递嵌入在程序集中的许可文件的名称
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// 文档目录的路径。
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 文档并获取第一个孩子
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // 文档目录的路径。
    // 加载 OneNote 文档并获取第一个孩子
}
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 文档目录的路径。
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// 文档目录的路径。
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// 加载 OneNote 文档
notebook.Save(dataDir);
```

```csharp
// 获取第一页
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

```csharp
// 加载 OneNote 文档
string dataDir = RunExamples.GetDataDir_NoteBook();

// 获取第一页
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// 文档目录的路径。
notebook.Save(dataDir, notebookSaveOptions);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 文档目录的路径。
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// 保存笔记本
notebook.Save(dataDir, notebookSaveOptions);
```

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "test.onetoc2");

// 加载 OneNote 笔记本
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // 文档目录的路径。
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// 加载 OneNote 笔记本
notebook.Save(dataDir);
```

```csharp
// 保存笔记本
// 文档目录的路径。
// 加载 OneNote 笔记本
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// 保存笔记本
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // 默认情况下，子加载是“惰性的”。
}
```

```csharp
// 子文档的实际加载只发生在这里。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // 对子文档做一些事情
        }
        else if (notebookChildNode is Notebook)
        {
            // 文档目录的路径。
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

显示如何以 pdf 格式保存笔记本。

显示如何将笔记本保存为图像。

显示如何从笔记本中获取所有文本。

显示如何以 pdf 格式保存扁平化的笔记本。

展示了如何遍历笔记本的文档以延迟加载它们。

显示如何将新分区添加到笔记本。

显示如何从流中加载笔记本。

显示如何加密笔记本。

显示如何使用指定选项将笔记本保存为图像。

显示如何将扁平笔记本保存为图像。

显示如何从笔记本中删除部分。

显示如何遍历笔记本的预加载文档。

显示如何传递笔记本的内容。

### 也可以看看

* interface [INotebookChildNode](../inotebookchildnode)
* 命名空间 [Aspose.Note](../../aspose.note)
* 部件 [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
