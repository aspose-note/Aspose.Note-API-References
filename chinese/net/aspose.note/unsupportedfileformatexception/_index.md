---
title: Class UnsupportedFileFormatException
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.UnsupportedFileFormatException 班级. 在文档加载期间抛出当 Aspose.Note 无法识别或不支持文件格式时抛出
type: docs
weight: 990
url: /zh/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

在文档加载期间抛出，当 Aspose.Note 无法识别或不支持文件格式时抛出。

```csharp
public class UnsupportedFileFormatException : Exception
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | 如果检测到，获取传递数据的文件格式。 |

### 例子

显示如何检查文档加载是否因不支持 OneNote 2007 格式而失败。

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

### 也可以看看

* 命名空间 [Aspose.Note](../../aspose.note/)
* 部件 [Aspose.Note](../../)


