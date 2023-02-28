---
title: Class OneSaveOptions
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Saving.OneSaveOptions クラス. ドキュメントを OneNote 形式で保存するときに追加オプションを指定できます
type: docs
weight: 810
url: /ja/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

ドキュメントを OneNote 形式で保存するときに追加オプションを指定できます。

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | デフォルトのコンストラクター。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | ドキュメント コンテンツを暗号化するためのパスワードを取得または設定します。 |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | 保存中に使用されるフォントの設定を取得または設定します |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | 保存するページ数を取得または設定します。デフォルトではMaxValue は、ドキュメントのすべてのページがレンダリングされることを意味します. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | 保存する最初のページのインデックスを取得または設定します。デフォルトは 0. です |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | ドキュメントの保存形式を取得します。 |

### 例

ドキュメントを暗号化して保存する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

OneSaveOptions を使用してドキュメントを保存する方法を示します。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### 関連項目

* class [SaveOptions](../saveoptions/)
* 名前空間 [Aspose.Note.Saving](../../aspose.note.saving/)
* 組み立て [Aspose.Note](../../)


