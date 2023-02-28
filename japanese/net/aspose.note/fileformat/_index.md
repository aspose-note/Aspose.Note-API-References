---
title: Enum FileFormat
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.FileFormat 列挙. OneNote ファイル形式を表します
type: docs
weight: 90
url: /ja/net/aspose.note/fileformat/
---
## FileFormat enumeration

OneNote ファイル形式を表します。

```csharp
public enum FileFormat
```

### 値

| 名前 | 価値 | 説明 |
| --- | --- | --- |
| Unknown | `0` | 不明なファイル形式です。 |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote オンライン. |

### 例

OneNote 2007 形式がサポートされていないためにドキュメントの読み込みが失敗したかどうかを確認する方法を示します。

```csharp
// ドキュメント ディレクトリへのパス。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

### 関連項目

* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


