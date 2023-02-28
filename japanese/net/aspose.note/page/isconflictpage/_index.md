---
title: Page.IsConflictPage
second_title: Aspose.Note for .NET API リファレンス
description: Page 財産. このページが競合ページかどうかを示す値を取得または設定します
type: docs
weight: 50
url: /ja/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

このページが競合ページかどうかを示す値を取得または設定します。

```csharp
public bool IsConflictPage { get; set; }
```

### 備考

2 人のユーザーが同じコンテンツを更新しようとすると、競合ページが発生します. この場合、最初のユーザーの変更は通常どおりに書き込まれます. ただし、別のユーザーの変更はマージできません. したがって、ページのコピーのみが作成されます競合としてマークされています.

このバージョンでは、競合は最初のユーザーの変更を優先して解決されます. したがって、ドキュメントに競合ページがある場合、それらは履歴に表示されますが、保存時にスキップされます. このフラグをリセットして、このページを保存することができます。いつものように歴史に。

競合ページによる操作の詳細なサンプルは、オンライン ドキュメントにあります。

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

* class [Page](../)
* 名前空間 [Aspose.Note](../../page/)
* 組み立て [Aspose.Note](../../../)


