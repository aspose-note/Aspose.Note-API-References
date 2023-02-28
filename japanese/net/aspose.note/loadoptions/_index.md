---
title: Class LoadOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.LoadOptions クラス. ドキュメントの読み込みに使用されるオプション
type: docs
weight: 320
url: /ja/net/aspose.note/loadoptions/
---
## LoadOptions class

ドキュメントの読み込みに使用されるオプション。

```csharp
public class LoadOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [LoadOptions](loadoptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DocumentPassword](../../aspose.note/loadoptions/documentpassword/) { get; set; } | 暗号化されたドキュメント コンテンツのパスワードを取得または設定します。ドキュメントがパスワードで保護されていない場合、値は無視されます. |
| [LoadHistory](../../aspose.note/loadoptions/loadhistory/) { get; set; } | ドキュメント ローダーが履歴を無視するかどうかを示す値を取得または設定します。 このオプションを使用して、メモリと CPU の使用率を減らします。 デフォルト値は次のとおりです。`真実`. |

### 例

ドキュメントを暗号化する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

ノートブックを暗号化する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
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

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


