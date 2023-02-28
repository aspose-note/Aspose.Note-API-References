---
title: Document.FileFormat
second_title: Aspose.Note for .NET API リファレンス
description: Document 財産. ファイル形式を取得します OneNote 2010OneNote Online.
type: docs
weight: 60
url: /ja/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

ファイル形式を取得します (OneNote 2010、OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

### 例

ドキュメントのファイル形式を取得する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // OneNote 2010 の処理
        break;
    case FileFormat.OneNoteOnline:
        // OneNote をオンラインで処理する
        break;
}
```

### 関連項目

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* 名前空間 [Aspose.Note](../../document/)
* 組み立て [Aspose.Note](../../../)


