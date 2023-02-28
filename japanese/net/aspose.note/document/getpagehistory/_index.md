---
title: Document.GetPageHistory
second_title: Aspose.Note for .NET API リファレンス
description: Document 方法. を取得しますPageHistoryこれにはドキュメントに表示された各ページの完全な履歴が含まれています 最も古いインデックス 0. 現在のページのリビジョンには次のようにアクセスできますCurrent履歴バージョンのコレクションとは別に含まれています.
type: docs
weight: 100
url: /ja/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

を取得します[`PageHistory`](../../pagehistory/)これには、ドキュメントに表示された各ページの完全な履歴が含まれています (最も古いインデックス 0). 現在のページのリビジョンには、次のようにアクセスできます。[`Current`](../../pagehistory/current/)履歴バージョンのコレクションとは別に含まれています.

```csharp
public PageHistory GetPageHistory(Page page)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| page | Page | ページの現在のリビジョン。 |

### 戻り値

[`PageHistory`](../../pagehistory/).

### 例

ページの以前のバージョンを復元する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込み、最初の子を取得します           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

ページの履歴を編集する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込み、最初の子を取得します           
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

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)


