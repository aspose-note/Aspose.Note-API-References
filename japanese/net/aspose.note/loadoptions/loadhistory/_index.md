---
title: LoadOptions.LoadHistory
second_title: Aspose.Note for .NET API リファレンス
description: LoadOptions 財産. ドキュメント ローダーが履歴を無視するかどうかを示す値を取得または設定します このオプションを使用してメモリと CPU の使用率を減らします デフォルト値は次のとおりです真実.
type: docs
weight: 30
url: /ja/net/aspose.note/loadoptions/loadhistory/
---
## LoadOptions.LoadHistory property

ドキュメント ローダーが履歴を無視するかどうかを示す値を取得または設定します。 このオプションを使用して、メモリと CPU の使用率を減らします。 デフォルト値は次のとおりです。`真実`.

```csharp
public bool LoadHistory { get; set; }
```

### 例

ページの履歴を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込む
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 最初のページを取得
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### 関連項目

* class [LoadOptions](../)
* 名前空間 [Aspose.Note](../../loadoptions/)
* 組み立て [Aspose.Note](../../../)


