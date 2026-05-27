---
title: "UnsupportedFileFormatException.FileFormat"
second_title: "Aspose.Note for .NET API 参考"
description: "UnsupportedFileFormatException 属性。获取已检测的传入数据的文件格式"
type: docs
weight: 10
url: /zh/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

如果检测到，则获取传入数据的文件格式。

```csharp
public FileFormat FileFormat { get; }
```

## 示例

展示如何检查文档加载是否因不支持 OneNote 2007 格式而失败。

```csharp
// 文档目录的路径。
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

### 另请参阅

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* namespace [Aspose.Note](../../unsupportedfileformatexception/)
* assembly [Aspose.Note](../../../)


