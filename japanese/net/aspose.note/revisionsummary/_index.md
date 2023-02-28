---
title: Class RevisionSummary
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.RevisionSummary クラス. ノードのリビジョンの概要を表します
type: docs
weight: 520
url: /ja/net/aspose.note/revisionsummary/
---
## RevisionSummary class

ノードのリビジョンの概要を表します。

```csharp
public class RevisionSummary
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [RevisionSummary](revisionsummary/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [AuthorMostRecent](../../aspose.note/revisionsummary/authormostrecent/) { get; set; } | 最新の作成者を取得または設定します。 |
| [LastModifiedTime](../../aspose.note/revisionsummary/lastmodifiedtime/) { get; set; } | 最終変更時刻を取得または設定します。 |

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

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


