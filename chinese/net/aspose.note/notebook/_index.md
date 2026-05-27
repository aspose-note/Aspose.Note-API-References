---
title: "类 Notebook"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Notebook 类。表示一个 Aspose.Note 笔记本"
type: docs
weight: 480
url: /zh/net/aspose.note/notebook/
---
## Notebook class

表示一个 Aspose.Note 笔记本。

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Notebook](notebook/#constructor)() | 初始化 `Notebook` 类的新实例。 |
| [Notebook](notebook/#constructor_1)(Stream) | 初始化 `Notebook` 类的新实例。从流中打开现有的 OneNote 笔记本。 |
| [Notebook](notebook/#constructor_3)(string) | 初始化 `Notebook` 类的新实例。从文件中打开现有的 OneNote 笔记本。 |
| [Notebook](notebook/#constructor_2)(Stream, NotebookLoadOptions) | 初始化 `Notebook` 类的新实例。从流中打开现有的 OneNote 笔记本。允许指定额外的加载选项。 |
| [Notebook](notebook/#constructor_4)(string, NotebookLoadOptions) | 初始化 `Notebook` 类的新实例。从文件中打开现有的 OneNote 笔记本。允许指定额外的选项，例如子项加载策略（\"lazy\"/instant）。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Color](../../aspose.note/notebook/color/) { get; set; } | 获取或设置颜色。 |
| [Count](../../aspose.note/notebook/count/) { get; } | 获取 `Notebook` 中包含的元素数量。 |
| [DisplayName](../../aspose.note/notebook/displayname/) { get; set; } | 获取或设置显示名称。 |
| [FileFormat](../../aspose.note/notebook/fileformat/) { get; } | 获取文件格式（OneNote 2010，OneNote Online）。 |
| [Guid](../../aspose.note/notebook/guid/) { get; } | 获取对象的全局唯一标识符。 |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled/) { get; set; } | 获取或设置指示是否启用历史记录的值。 |
| [Item](../../aspose.note/notebook/item/) { get; } | 通过给定索引获取笔记本子节点。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild/)(INotebookChildNode) | 将节点添加到列表末尾。 |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes/)() | 按节点类型获取所有子节点。 |
| [GetEnumerator](../../aspose.note/notebook/getenumerator/)() | 返回一个枚举器，用于遍历 `Notebook` 的子节点。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument)(Stream) | 添加子文档节点。从流中打开现有的 OneNote 文档。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_2)(string) | 添加子文档节点。从文件中打开现有的 OneNote 文档。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_1)(Stream, LoadOptions) | 添加子文档节点。从流中打开现有的 OneNote 文档。允许指定额外的加载选项。 |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_3)(string, LoadOptions) | 添加子文档节点。从文件中打开现有的 OneNote 文档。允许指定额外的加载选项。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook)(Stream) | 添加子笔记本节点。从流中打开现有的 OneNote 笔记本。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_2)(string) | 添加子笔记本节点。从文件中打开现有的 OneNote 笔记本。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_1)(Stream, NotebookLoadOptions) | 添加子笔记本节点。从流中打开现有的 OneNote 笔记本。允许指定额外的加载选项。 |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_3)(string, NotebookLoadOptions) | 添加子笔记本节点。从文件中打开现有的 OneNote 笔记本。允许指定额外的加载选项。 |
| [RemoveChild](../../aspose.note/notebook/removechild/)(INotebookChildNode) | 移除子节点。 |
| [Save](../../aspose.note/notebook/save/#save)(Stream) | 将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/notebook/save/#save_3)(string) | 将 OneNote 文档保存到文件中。 |
| [Save](../../aspose.note/notebook/save/#save_2)(Stream, NotebookSaveOptions) | 使用指定的保存选项将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/notebook/save/#save_1)(Stream, SaveFormat) | 以指定格式将 OneNote 文档保存到流中。 |
| [Save](../../aspose.note/notebook/save/#save_5)(string, NotebookSaveOptions) | 使用指定的保存选项将 OneNote 文档保存到文件中。 |
| [Save](../../aspose.note/notebook/save/#save_4)(string, SaveFormat) | 以指定格式将 OneNote 文档保存到文件中。 |

## 示例

展示如何保存笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// 保存笔记本
notebook.Save(dataDir);
```

展示如何以 PDF 格式保存笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// 保存笔记本
notebook.Save(dataDir);
```

展示如何将笔记本保存为图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// 保存笔记本
notebook.Save(dataDir);
```

展示如何获取笔记本中的所有文本。

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

展示如何遍历笔记本的文档并懒加载它们。

```csharp
string inputFile = "Notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// 默认情况下，子项加载为“懒惰”。
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // 子文档的实际加载仅在此处进行。
    // 对子文档进行操作
}
```

展示如何向笔记本添加新章节。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

// 向笔记本追加新子项
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// 保存笔记本
notebook.Save(dataDir);
```

展示如何从流加载笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notebook.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

展示如何打开加密的笔记本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
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

展示如何从笔记本中删除章节。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

// 加载 OneNote 笔记本
var notebook = new Notebook(dataDir + "test.onetoc2");

// 遍历其子节点以搜索所需的子项
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // 从笔记本中删除子项
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// 保存笔记本
notebook.Save(dataDir);
```

展示如何遍历笔记本的预加载文档。

```csharp
// 默认情况下，子项加载为“懒惰”。
// 因此，已完成即时加载，
// 需要设置 NotebookLoadOptions.InstantLoading 标志。
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notebook.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// 所有子文档已加载。
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // 对子文档进行操作
}
```

展示如何遍历笔记本的内容。

```csharp
// 文档目录的路径。
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
            // 对子文档进行操作
        }
        else if (notebookChildNode is Notebook)
        {
            // 对子笔记本进行操作
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### 另请参阅

* interface [INotebookChildNode](../inotebookchildnode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


