---
title: "LoadOptions.LoadHistory"
second_title: "Aspose.Note for .NET API 参考"
description: "LoadOptions 属性。获取或设置一个值，指示文档加载器是否应忽略历史记录。使用此选项可降低内存和 CPU 使用率。默认值为 true"
type: docs
weight: 30
url: /zh/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

获取或设置一个值，指示文档加载器是否应忽略历史记录。使用此选项可降低内存和 CPU 使用率。默认值为 `true`。

```csharp
public bool LoadHistory { get; set; }
```

## 示例

展示如何获取页面的历史记录。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 获取第一页
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### 另请参阅

* class [LoadOptions](../)
* namespace [Aspose.Note](../../loadoptions/)
* assembly [Aspose.Note](../../../)


