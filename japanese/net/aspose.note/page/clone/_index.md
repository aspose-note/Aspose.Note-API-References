---
title: Page.Clone
second_title: Aspose.Note for .NET API リファレンス
description: Page 方法. ページを複製します
type: docs
weight: 140
url: /ja/net/aspose.note/page/clone/
---
## Page.Clone method

ページを複製します。

```csharp
public Page Clone(bool cloneHistory = false)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| cloneHistory | Boolean | ページの履歴を複製するかどうかを指定します.. |

### 戻り値

ページの複製。

### 例

ページの現在のバージョンを履歴にプッシュする方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込み、最初の子を取得します           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

ページを複製する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote ドキュメントを読み込む
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 履歴なしで新しいドキュメントにクローンします
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// 履歴付きの新しいドキュメントにクローンします
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### 関連項目

* class [Page](../)
* 名前空間 [Aspose.Note](../../page/)
* 組み立て [Aspose.Note](../../../)


