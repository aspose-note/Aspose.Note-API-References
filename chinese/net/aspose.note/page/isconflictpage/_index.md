---
title: "Page.IsConflictPage"
second_title: "Aspose.Note for .NET API 参考"
description: "Page 属性。获取或设置一个值，指示此页面是否为冲突页面"
type: docs
weight: 50
url: /zh/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

获取或设置一个值，指示此页面是否为冲突页面。

```csharp
public bool IsConflictPage { get; set; }
```

## 备注

冲突页面在两个用户尝试更新相同内容时产生。在这种情况下，第一位用户的更改会正常写入，但另一位用户的更改无法合并。因此会创建页面的副本并标记为冲突。

在此版本中，冲突会以第一位用户的更改为准进行解决。因此，如果文档中存在冲突页面，它们会在历史记录中显示，但在保存时会被跳过。可以重置此标志，以便将这些页面像普通页面一样保存到历史记录中。

有关冲突页面操作的详细示例可在在线文档中找到。

## 示例

展示如何检查页面是否为冲突页面（即它包含 OneNote 无法自动合并的更改）。

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

    // 默认情况下，冲突页面在保存时会被跳过。
    // 如果将其标记为非冲突，则它将在历史记录中像普通页面一样保存。
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### 另请参阅

* class [Page](../)
* namespace [Aspose.Note](../../page/)
* assembly [Aspose.Note](../../../)


