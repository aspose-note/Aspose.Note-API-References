---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note for .NET API リファレンス
description: UnsupportedFileFormatException 財産. 検出された場合渡されたデータのファイル形式を取得します
type: docs
weight: 10
url: /ja/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

検出された場合、渡されたデータのファイル形式を取得します。

```csharp
public FileFormat FileFormat { get; }
```

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

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* 名前空間 [Aspose.Note](../../unsupportedfileformatexception/)
* 組み立て [Aspose.Note](../../../)


