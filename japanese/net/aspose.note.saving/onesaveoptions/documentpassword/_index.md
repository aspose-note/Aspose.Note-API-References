---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note for .NET API リファレンス
description: OneSaveOptions 財産. ドキュメント コンテンツを暗号化するためのパスワードを取得または設定します
type: docs
weight: 20
url: /ja/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

ドキュメント コンテンツを暗号化するためのパスワードを取得または設定します。

```csharp
public string DocumentPassword { get; set; }
```

### 例

ドキュメントを暗号化して保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### 関連項目

* class [OneSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../onesaveoptions/)
* 組み立て [Aspose.Note](../../../)


