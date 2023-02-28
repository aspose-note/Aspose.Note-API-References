---
title: Class UnsupportedFileFormatException
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.UnsupportedFileFormatException クラス. ファイル フォーマットが認識されないかAspose.Note. でサポートされていない場合ドキュメントのロード中にスローされます
type: docs
weight: 990
url: /ja/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

ファイル フォーマットが認識されないか、Aspose.Note. でサポートされていない場合、ドキュメントのロード中にスローされます。

```csharp
public class UnsupportedFileFormatException : Exception
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | 検出された場合、渡されたデータのファイル形式を取得します。 |

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


