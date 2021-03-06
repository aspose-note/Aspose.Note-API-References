---
title: LoadHistory
second_title: Aspose.Note for .NET API 参考
description: 获取或设置一个值该值指示文档加载器是否应忽略历史记录 使用此选项可减少内存和 CPU 使用率 默认值为 true 
type: docs
weight: 30
url: /zh/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

获取或设置一个值，该值指示文档加载器是否应忽略历史记录。 使用此选项可减少内存和 CPU 使用率。 默认值为` true` 。

```csharp
public bool LoadHistory { get; set; }
```

### 例子

显示如何获取页面的历史记录。

```csharp
// 通过文件路径加载图片。
string dataDir = RunExamples.GetDataDir_Pages();

// 设置图像对齐
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 添加图片
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

### 也可以看看

* class [LoadOptions](../../loadoptions)
* 命名空间 [Aspose.Note](../../loadoptions)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
