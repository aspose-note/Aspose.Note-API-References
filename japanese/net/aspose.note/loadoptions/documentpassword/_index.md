---
title: LoadOptions.DocumentPassword
second_title: Aspose.Note for .NET API リファレンス
description: LoadOptions 財産. 暗号化されたドキュメント コンテンツのパスワードを取得または設定しますドキュメントがパスワードで保護されていない場合値は無視されます.
type: docs
weight: 20
url: /ja/net/aspose.note/loadoptions/documentpassword/
---
## LoadOptions.DocumentPassword property

暗号化されたドキュメント コンテンツのパスワードを取得または設定します。ドキュメントがパスワードで保護されていない場合、値は無視されます.

```csharp
public string DocumentPassword { get; set; }
```

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

### 関連項目

* class [LoadOptions](../)
* 名前空間 [Aspose.Note](../../loadoptions/)
* 組み立て [Aspose.Note](../../../)


