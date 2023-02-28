---
title: CompositeNode1.FirstChild
second_title: Aspose.Note for .NET API リファレンス
description: CompositeNode 財産. このノードの最初の子ノードを取得します
type: docs
weight: 10
url: /ja/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

このノードの最初の子ノードを取得します。

```csharp
public T FirstChild { get; }
```

### 例

ページが競合ページ (つまり、OneNote が自動的にマージできなかった変更がある) であるかどうかを確認する方法を示します。

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込む
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

    // デフォルトでは、競合ページは保存時にスキップされます。
    // 非競合としてマークすると、通常の履歴として保存されます。
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### 関連項目

* class [CompositeNode&lt;T&gt;](../)
* 名前空間 [Aspose.Note](../../compositenode-1/)
* 組み立て [Aspose.Note](../../../)


