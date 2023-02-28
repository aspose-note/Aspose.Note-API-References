---
title: AttachedFile.Bytes
second_title: Aspose.Note for .NET API 参考
description: AttachedFile 财产. 获取嵌入式文件的二进制数据
type: docs
weight: 50
url: /zh/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

获取嵌入式文件的二进制数据。

```csharp
public byte[] Bytes { get; }
```

### 例子

显示如何获取附加文件的内容。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Attachments();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Sample1.one");

// 获取附加文件节点列表
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

//遍历所有节点
foreach (AttachedFile file in nodes)
{
    // 将附加文件加载到流对象
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // 创建本地文件
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // 复制文件流
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### 也可以看看

* class [AttachedFile](../)
* 命名空间 [Aspose.Note](../../attachedfile/)
* 部件 [Aspose.Note](../../../)


