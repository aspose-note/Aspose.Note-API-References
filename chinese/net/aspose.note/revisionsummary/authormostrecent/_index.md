---
title: RevisionSummary.AuthorMostRecent
second_title: Aspose.Note for .NET API 参考
description: RevisionSummary 财产. 获取或设置最近的作者
type: docs
weight: 20
url: /zh/net/aspose.note/revisionsummary/authormostrecent/
---
## RevisionSummary.AuthorMostRecent property

获取或设置最近的作者。

```csharp
public string AuthorMostRecent { get; set; }
```

### 例子

显示如何编辑页面的元信息。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档并获取第一个子节点           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// 阅读此页面的内容修订摘要
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// 更新此页面的页面修订摘要
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

显示如何检查页面是否为冲突页面（即它具有 OneNote 无法自动合并的更改）。

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档
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

    // 默认情况下，冲突页面只是在保存时被跳过。
    // 如果将其标记为非冲突，则它将照常保存在历史记录中。
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### 也可以看看

* class [RevisionSummary](../)
* 命名空间 [Aspose.Note](../../revisionsummary/)
* 部件 [Aspose.Note](../../../)


