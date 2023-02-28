---
title: Document.GetPageHistory
second_title: Aspose.Note for .NET API 参考
description: Document 方法. 获取PageHistory其中包含文档中出现的每个页面的完整历史记录最早的索引为 0 当前页面修订可以访问为Current并与历史版本的集合分开包含
type: docs
weight: 100
url: /zh/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

获取[`PageHistory`](../../pagehistory/)其中包含文档中出现的每个页面的完整历史记录（最早的索引为 0）。 当前页面修订可以访问为[`Current`](../../pagehistory/current/)并与历史版本的集合分开包含。

```csharp
public PageHistory GetPageHistory(Page page)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| page | Page | 页面的当前修订版。 |

### 返回值

的[`PageHistory`](../../pagehistory/).

### 例子

显示如何恢复页面的先前版本。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档并获取第一个子节点           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

显示如何编辑页面的历史记录。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档并获取第一个子节点           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
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

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* 命名空间 [Aspose.Note](../../document/)
* 部件 [Aspose.Note](../../../)


