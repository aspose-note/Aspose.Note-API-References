---
title: Page.IsConflictPage
second_title: Aspose.Note for .NET API 参考
description: Page 财产. 获取或设置一个值该值指示此页是否为冲突页
type: docs
weight: 50
url: /zh/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

获取或设置一个值，该值指示此页是否为冲突页。

```csharp
public bool IsConflictPage { get; set; }
```

### 评论

当两个用户尝试更新相同的内容时出现冲突页面。 在这种情况下，第一个用户的更改照常写入。 但是无法合并另一个用户的更改。 所以只创建了一个页面副本并标记为冲突.

在此版本中，冲突得到解决，有利于第一个用户的更改。 因此，如果文档有冲突页面，那么它们将显示在历史记录中，但在保存时将被跳过。 可以重置此标志以保存此页面像往常一样在历史上.

通过冲突页面操作的详细示例可以在在线文档中找到。

### 例子

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

* class [Page](../)
* 命名空间 [Aspose.Note](../../page/)
* 部件 [Aspose.Note](../../../)


