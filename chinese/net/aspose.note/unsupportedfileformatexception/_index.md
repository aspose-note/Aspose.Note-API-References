---
title: "UnsupportedFileFormatException 类"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.UnsupportedFileFormatException 类。在文档加载期间抛出，当文件格式未被识别或不受 Aspose.Note 支持时"
type: docs
weight: 1070
url: /zh/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

在文档加载期间抛出，当文件格式未被识别或不受 Aspose.Note 支持时。

```csharp
public class UnsupportedFileFormatException : Exception
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | 如果检测到，则获取传入数据的文件格式。 |

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

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


