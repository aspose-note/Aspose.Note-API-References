---
title: Enum FileFormat
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.FileFormat 枚举. 代表OneNote文件格式
type: docs
weight: 90
url: /zh/net/aspose.note/fileformat/
---
## FileFormat enumeration

代表OneNote文件格式。

```csharp
public enum FileFormat
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| Unknown | `0` | 未知文件格式。 |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote Online. |

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


