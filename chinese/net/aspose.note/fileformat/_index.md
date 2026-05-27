---
title: "枚举 FileFormat"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.FileFormat 枚举。表示 OneNote 文件格式"
type: docs
weight: 90
url: /zh/net/aspose.note/fileformat/
---
## FileFormat enumeration

表示 OneNote 文件格式。

```csharp
public enum FileFormat
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Unknown | `0` | 未知文件格式。 |
| OneNote2007 | `1` | OneNote 2010。 |
| OneNote2010 | `2` | OneNote 2010。 |
| OneNoteOnline | `3` | OneNote Online。 |

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


