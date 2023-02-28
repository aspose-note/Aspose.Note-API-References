---
title: Page.PageContentRevisionSummary
second_title: Aspose.Note for .NET API リファレンス
description: Page 財産. ページとその子ノードの改訂概要を取得または設定します
type: docs
weight: 90
url: /ja/net/aspose.note/page/pagecontentrevisionsummary/
---
## Page.PageContentRevisionSummary property

ページとその子ノードの改訂概要を取得または設定します。

```csharp
public RevisionSummary PageContentRevisionSummary { get; set; }
```

### 例

ページのメタ情報を編集する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込み、最初の子を取得します           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// このページのコンテンツ リビジョン サマリーの読み取り
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// このページのページ リビジョン サマリーを更新します
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

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

* class [RevisionSummary](../../revisionsummary/)
* class [Page](../)
* 名前空間 [Aspose.Note](../../page/)
* 組み立て [Aspose.Note](../../../)


