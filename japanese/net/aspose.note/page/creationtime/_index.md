---
title: Page.CreationTime
second_title: Aspose.Note for .NET API リファレンス
description: Page 財産. 作成時刻を取得または設定します
type: docs
weight: 40
url: /ja/net/aspose.note/page/creationtime/
---
## Page.CreationTime property

作成時刻を取得または設定します。

```csharp
public DateTime CreationTime { get; set; }
```

### 例

ページに関するメタ情報を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// ドキュメントを Aspose.Note にロードします。
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

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

* class [Page](../)
* 名前空間 [Aspose.Note](../../page/)
* 組み立て [Aspose.Note](../../../)


