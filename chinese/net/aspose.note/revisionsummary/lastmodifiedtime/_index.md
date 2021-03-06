---
title: LastModifiedTime
second_title: Aspose.Note for .NET API 参考
description: 获取或设置最后修改时间
type: docs
weight: 30
url: /zh/net/aspose.note/revisionsummary/lastmodifiedtime/
---
## RevisionSummary.LastModifiedTime property

获取或设置最后修改时间。

```csharp
public DateTime LastModifiedTime { get; set; }
```

### 例子

显示如何编辑页面的元信息。

```csharp
// 在输出屏幕上打印文本
string dataDir = RunExamples.GetDataDir_Pages();

// 文档目录的路径。           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// 将文档加载到 Aspose.Note。
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// 获取所有富文本节点
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// 替换形状的文本
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // 保存为任何支持的文件格式
    // 文档目录的路径。
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

显示如何检查页面是否为冲突页面（即它具有 OneNote 无法自动合并的更改）。

### 也可以看看

* class [RevisionSummary](../../revisionsummary)
* 命名空间 [Aspose.Note](../../revisionsummary)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
